---
-api-id: T:Windows.Graphics.DirectX.Direct3D11.IDirect3DSurface
-api-type: winrt interface
---

<!-- Interface syntax.
public interface IDirect3DSurface : Windows.Foundation.IClosable
-->

# Windows.Graphics.DirectX.Direct3D11.IDirect3DSurface

## -description
This represents an [IDXGISurface](http://msdn.microsoft.com/library/9210b966-9e9a-4cd1-ba70-6f1a9fda9d80) and can be used to interop between Windows Runtime components that need to exchange [IDXGISurface](http://msdn.microsoft.com/library/9210b966-9e9a-4cd1-ba70-6f1a9fda9d80) references.

## -remarks
To move back and forth between [IDirect3DSurface](idirect3dsurface.md) and [IDXGISurface](http://msdn.microsoft.com/library/9210b966-9e9a-4cd1-ba70-6f1a9fda9d80), use the [CreateDirect3DSurface](createdirect3dsurface.md) and [GetDXGIInterface(IDirect3DSurface^, DXGIType**)](getdxgiinterface_2.md) functions.

## -examples
First include the necessary headers and namespaces:

```cpp
#include <Windows.Graphics.DirectX.Direct3D11.interop.h>
#include <dxgi.h>
using namespace Windows::Graphics::DirectX::Direct3D11;
using namespace Microsoft::WRL;
```

To get the native DirectX surface that is wrapped by a Direct3DSurface:

```cpp
IDirect3DSurface^ d3dSurface = ...;  
ComPtr<IDXGISurface> nativeSurface;
HRESULT hr = GetDXGIInterface(d3dSurface, nativeSurface.GetAddressOf());
```

To create a new Direct3DSurface object wrapping a native DirectX surface:

```cpp
ComPtr<IDXGISurface> nativeSurface = ...;
IDirect3DSurface^ d3dSurface = CreateDirect3DSurface(nativeSurface.Get());

```



## -see-also
[IClosable](../windows.foundation/iclosable.md)