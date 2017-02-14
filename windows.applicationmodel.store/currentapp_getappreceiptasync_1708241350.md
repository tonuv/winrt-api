---
-api-id: M:Windows.ApplicationModel.Store.CurrentApp.GetAppReceiptAsync
-api-type: winrt method
---

<!-- Method syntax
public Windows.Foundation.IAsyncOperation<string> GetAppReceiptAsync()
-->

# Windows.ApplicationModel.Store.CurrentApp.GetAppReceiptAsync

## -description
Requests all receipts for the purchase of the app and any in-app products. For examples of how receipt information can be used, see [Using receipts to verify product purchases](https://msdn.microsoft.com/windows/uwp/monetize/use-receipts-to-verify-product-purchases).

## -returns
An XML-formatted string that contains all receipt information for the purchase of the app and any in-app products.

## -remarks
For more information about the contents of the receipt, see [Using receipts to verify product purchases](https://msdn.microsoft.com/windows/uwp/monetize/use-receipts-to-verify-product-purchases).

Calling this method does not need network connectivity, but if the user is signed off from the store then calling this will throw System.Exception (HRESULT: 0x80070525) "The specified account does not exist."

## -examples

## -see-also
