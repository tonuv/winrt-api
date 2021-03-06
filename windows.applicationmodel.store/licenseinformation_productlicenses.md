---
-api-id: P:Windows.ApplicationModel.Store.LicenseInformation.ProductLicenses
-api-type: winrt property
---

<!-- Property syntax
public Windows.Foundation.Collections.IMapView<string, Windows.ApplicationModel.Store.ProductLicense> ProductLicenses { get; }
-->

# Windows.ApplicationModel.Store.LicenseInformation.ProductLicenses

## -description
Gets the associative list of licenses for in-app products that a user is currently entitled to.

> [!IMPORTANT]
> The returned list of [ProductLicense](productlicense.md) objects will always represent all in-app products that a user is currently entitled to (**isActive = true**). However, this list may or may not also contain [ProductLicense](productlicense.md) objects for products that a user is not currently entitled to (**isActive = false**).

Call [ProductLicense.isActive](productlicense_isactive.md) to determine if a user is entitled to an in-app product.

## -property-value
The associative list of feature licenses.

## -remarks

## -examples

## -see-also
