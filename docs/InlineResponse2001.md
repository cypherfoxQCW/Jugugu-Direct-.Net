
# Org.OpenAPITools.Model.InlineResponse2001

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**State** | **string** | 响应状态分为：-1,0,1 分别代表响应错误、响应提示、响应成功 | 
**Msg** | **string** | 响应状态为-1时该值为错误信息。响应状态为0时，该值为响应提示信息。响应状态为1时该值为空字符串 | 
**Phone** | **string** |  | 
**Virifycodeid** | **string** | 验证码图片的ID值 | 
**Virifyimage** | **string** | data:image/png;base64 | 
**Confluxaddress** | **string** | 树图区块链地址 | 
**Ethaddress** | **string** | 以太坊、Arbitrum、polygon、BSC等EVM链地址 | 
**Token** | **string** | 用户登录识别令牌，用于后续多个函数的交互，作为输入参数 | 

[[Back to Model list]](../README.md#documentation-for-models)
[[Back to API list]](../README.md#documentation-for-api-endpoints)
[[Back to README]](../README.md)

