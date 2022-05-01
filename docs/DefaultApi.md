# Org.OpenAPITools.Api.DefaultApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**IsPhoneRegPost**](DefaultApi.md#isphoneregpost) | **POST** /IsPhoneReg | 检查手机号是否注册
[**JuguguLoginCodeandReturnInfoPost**](DefaultApi.md#jugugulogincodeandreturninfopost) | **POST** /Jugugu_LoginCodeandReturnInfo | ①获取验证码图片
[**JugugugRegAndVerifyandReturnInfoPost**](DefaultApi.md#jugugugregandverifyandreturninfopost) | **POST** /Jugugug_RegAndVerifyandReturnInfo | ③注册Jugugu



## IsPhoneRegPost

> InlineResponse200 IsPhoneRegPost (InlineObject inlineObject = null)

检查手机号是否注册

检查手机号是否注册，返回“true”和“false”字符串

### Example

```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Org.OpenAPITools.Api;
using Org.OpenAPITools.Client;
using Org.OpenAPITools.Model;

namespace Example
{
    public class IsPhoneRegPostExample
    {
        public static void Main()
        {
            Configuration.Default.BasePath = "http://localhost";
            var apiInstance = new DefaultApi(Configuration.Default);
            var inlineObject = new InlineObject(); // InlineObject |  (optional) 

            try
            {
                // 检查手机号是否注册
                InlineResponse200 result = apiInstance.IsPhoneRegPost(inlineObject);
                Debug.WriteLine(result);
            }
            catch (ApiException e)
            {
                Debug.Print("Exception when calling DefaultApi.IsPhoneRegPost: " + e.Message );
                Debug.Print("Status Code: "+ e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inlineObject** | [**InlineObject**](InlineObject.md)|  | [optional] 

### Return type

[**InlineResponse200**](InlineResponse200.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: */*

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 成功 |  -  |

[[Back to top]](#)
[[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## JuguguLoginCodeandReturnInfoPost

> InlineResponse2001 JuguguLoginCodeandReturnInfoPost (InlineObject2 inlineObject2 = null)

①获取验证码图片

获取用于防御机器人的验证码图片，phone的传参必须为空字符串

### Example

```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Org.OpenAPITools.Api;
using Org.OpenAPITools.Client;
using Org.OpenAPITools.Model;

namespace Example
{
    public class JuguguLoginCodeandReturnInfoPostExample
    {
        public static void Main()
        {
            Configuration.Default.BasePath = "http://localhost";
            var apiInstance = new DefaultApi(Configuration.Default);
            var inlineObject2 = new InlineObject2(); // InlineObject2 |  (optional) 

            try
            {
                // ①获取验证码图片
                InlineResponse2001 result = apiInstance.JuguguLoginCodeandReturnInfoPost(inlineObject2);
                Debug.WriteLine(result);
            }
            catch (ApiException e)
            {
                Debug.Print("Exception when calling DefaultApi.JuguguLoginCodeandReturnInfoPost: " + e.Message );
                Debug.Print("Status Code: "+ e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inlineObject2** | [**InlineObject2**](InlineObject2.md)|  | [optional] 

### Return type

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 成功 |  -  |

[[Back to top]](#)
[[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)


## JugugugRegAndVerifyandReturnInfoPost

> InlineResponse2001 JugugugRegAndVerifyandReturnInfoPost (InlineObject1 inlineObject1 = null)

③注册Jugugu

注册jugugu，注意三点 1.phone的传参必须为11位的国内手机号。 2.robotcodeid和robotcode是通过【①】获得 3.code短信验证码通过【②】 4.paymentpassword区块链短密钥，该密钥为用户进行链上交互使用，密钥设置长度>9位，且包含0-1 A-B a-b 已经特殊字符[~!@#$%^&*?_+;',./\\|·！￥（）{}：“《》？、，。；’”\"《》…-]+

### Example

```csharp
using System.Collections.Generic;
using System.Diagnostics;
using Org.OpenAPITools.Api;
using Org.OpenAPITools.Client;
using Org.OpenAPITools.Model;

namespace Example
{
    public class JugugugRegAndVerifyandReturnInfoPostExample
    {
        public static void Main()
        {
            Configuration.Default.BasePath = "http://localhost";
            var apiInstance = new DefaultApi(Configuration.Default);
            var inlineObject1 = new InlineObject1(); // InlineObject1 |  (optional) 

            try
            {
                // ③注册Jugugu
                InlineResponse2001 result = apiInstance.JugugugRegAndVerifyandReturnInfoPost(inlineObject1);
                Debug.WriteLine(result);
            }
            catch (ApiException e)
            {
                Debug.Print("Exception when calling DefaultApi.JugugugRegAndVerifyandReturnInfoPost: " + e.Message );
                Debug.Print("Status Code: "+ e.ErrorCode);
                Debug.Print(e.StackTrace);
            }
        }
    }
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inlineObject1** | [**InlineObject1**](InlineObject1.md)|  | [optional] 

### Return type

[**InlineResponse2001**](InlineResponse2001.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
| **200** | 成功 |  -  |

[[Back to top]](#)
[[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to Model list]](../README.md#documentation-for-models)
[[Back to README]](../README.md)

