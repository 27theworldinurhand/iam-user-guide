# Actions, Resources, and Condition Keys for AWS WAF<a name="list_awswaf"></a>

AWS WAF \(service prefix: `waf`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

References:
+ Learn how to [configure this service](https://docs.aws.amazon.com/waf/latest/developerguide/waf-chapter.html)\.
+ View a list of the [API operations available for this service](https://docs.aws.amazon.com/waf/latest/APIReference/API_Operations_AWS_WAF.html)\.
+ Learn how to secure this service and its resources by [using IAM](https://docs.aws.amazon.com/waf/latest/developerguide/waf-auth-and-access-control.html) permission policies\.

**Topics**
+ [Actions Defined by AWS WAF](#awswaf-actions-as-permissions)
+ [Resources Defined by AWS WAF](#awswaf-resources-for-iam-policies)
+ [Condition Keys for AWS WAF](#awswaf-policy-keys)

## Actions Defined by AWS WAF<a name="awswaf-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. Use policies to grant permissions to perform an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\.

The **Resource** column indicates whether each action supports resource\-level permissions\. If there is no value for this column, you must specify all resources \("\*"\) in the `Resource` element of your policy statement\. If the column includes a resource type, then you can specify an ARN of that type in a statement with that action\. Required resources are indicated in the table with an asterisk \(\*\)\. If you specify a resource\-level permission ARN in a statement using this action, then it must be of this type\. Some actions support multiple resource types\. If the resource type is optional \(not indicated as required\), then you can choose to use one but not the other\.

For details about the columns in the following table, see [The Actions Table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  
[\[See the AWS documentation website for more details\]](http://docs.aws.amazon.com/IAM/latest/UserGuide/list_awswaf.html)

## Resources Defined by AWS WAF<a name="awswaf-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#awswaf-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The Resource Types Table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource Types | ARN | Condition Keys | 
| --- | --- | --- | 
|   [ bytematchset ](https://docs.aws.amazon.com/waf/latest/APIReference/API_ByteMatchSet.html)  |  arn:$\{Partition\}:waf::$\{Account\}:bytematchset/$\{Id\}  |  | 
|   [ ipset ](https://docs.aws.amazon.com/waf/latest/APIReference/API_IPSet.html)  |  arn:$\{Partition\}:waf::$\{Account\}:ipset/$\{Id\}  |  | 
|   [ ratebasedrule ](https://docs.aws.amazon.com/waf/latest/APIReference/API_RateBasedRule.html)  |  arn:$\{Partition\}:waf::$\{Account\}:ratebasedrule/$\{Id\}  |   [ aws:ResourceTag/$\{TagKey\} ](#awswaf-aws_ResourceTag___TagKey_)   | 
|   [ rule ](https://docs.aws.amazon.com/waf/latest/APIReference/API_Rule.html)  |  arn:$\{Partition\}:waf::$\{Account\}:rule/$\{Id\}  |   [ aws:ResourceTag/$\{TagKey\} ](#awswaf-aws_ResourceTag___TagKey_)   | 
|   [ sizeconstraintset ](https://docs.aws.amazon.com/waf/latest/APIReference/API_SizeConstraintSet.html)  |  arn:$\{Partition\}:waf::$\{Account\}:sizeconstraintset/$\{Id\}  |  | 
|   [ sqlinjectionmatchset ](https://docs.aws.amazon.com/waf/latest/APIReference/API_SqlInjectionMatchSet.html)  |  arn:$\{Partition\}:waf::$\{Account\}:sqlinjectionmatchset/$\{Id\}  |  | 
|   [ webacl ](https://docs.aws.amazon.com/waf/latest/APIReference/API_WebACL.html)  |  arn:$\{Partition\}:waf::$\{Account\}:webacl/$\{Id\}  |   [ aws:ResourceTag/$\{TagKey\} ](#awswaf-aws_ResourceTag___TagKey_)   | 
|   [ xssmatchset ](https://docs.aws.amazon.com/waf/latest/APIReference/API_XssMatchSet.html)  |  arn:$\{Partition\}:waf::$\{Account\}:xssmatchset/$\{Id\}  |  | 
|   [ regexmatchset ](https://docs.aws.amazon.com/waf/latest/APIReference/API_RegexMatchSet.html)  |  arn:$\{Partition\}:waf::$\{Account\}:regexmatch/$\{Id\}  |  | 
|   [ regexpatternset ](https://docs.aws.amazon.com/waf/latest/APIReference/API_RegexPatternSet.html)  |  arn:$\{Partition\}:waf::$\{Account\}:regexpatternset/$\{Id\}  |  | 
|   [ geomatchset ](https://docs.aws.amazon.com/waf/latest/APIReference/API_GeoMatchSet.html)  |  arn:$\{Partition\}:waf::$\{Account\}:geomatchset/$\{Id\}  |  | 
|   [ rulegroup ](https://docs.aws.amazon.com/waf/latest/APIReference/API_RuleGroup.html)  |  arn:$\{Partition\}:waf::$\{Account\}:rulegroup/$\{Id\}  |   [ aws:ResourceTag/$\{TagKey\} ](#awswaf-aws_ResourceTag___TagKey_)   | 

## Condition Keys for AWS WAF<a name="awswaf-policy-keys"></a>

AWS WAF defines the following condition keys that can be used in the `Condition` element of an IAM policy\. You can use these keys to further refine the conditions under which the policy statement applies\. For details about the columns in the following table, see [The Condition Keys Table](reference_policies_actions-resources-contextkeys.md#context_keys_table)\.

To view the global condition keys that are available to all services, see [Available Global Condition Keys](reference_policies_condition-keys.html#AvailableKeys) in the *IAM Policy Reference*\.


****  

| Condition Keys | Description | Type | 
| --- | --- | --- | 
|   [ aws:RequestTag/$\{TagKey\} ](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_condition-keys.html#condition-keys-requesttag)  | Filters actions based on the allowed set of values for each of the tags | String | 
|   [ aws:ResourceTag/$\{TagKey\} ](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_condition-keys.html#condition-keys-resourcetag)  | Filters actions based on tag\-value assoicated with the resource | String | 
|   [ aws:TagKeys ](https://docs.aws.amazon.com/IAM/latest/UserGuide/reference_policies_condition-keys.html#condition-keys-tagkeys)  | Filters actions based on the presence of mandatory tags in the request | String | 