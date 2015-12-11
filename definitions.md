## Definitions
### AgentBean
|Name|Description|Required|Schema|Default|
|----|----|----|----|----|
|hostId||false|string||
|hostName||false|string||
|envId||false|string||
|deployId||false|string||
|deployStage||false|enum (UNKNOWN, PRE_DOWNLOAD, DOWNLOADING, POST_DOWNLOAD, STAGING, PRE_RESTART, RESTARTING, POST_RESTART, SERVING_BUILD)||
|state||false|enum (NORMAL, PAUSED_BY_SYSTEM, PAUSED_BY_USER, RESET, DELETE, UNREACHABLE)||
|status||false|enum (SUCCEEDED, UNKNOWN, AGENT_FAILED, RETRYABLE_AGENT_FAILED, SCRIPT_FAILED, ABORTED_BY_SERVICE, SCRIPT_TIMEOUT, TOO_MANY_RETRY, RUNTIME_MISMATCH)||
|startDate||false|integer (int64)||
|lastUpdateDate||false|integer (int64)||
|lastOperator||false|string||
|lastErrno||false|integer (int32)||
|failCount||false|integer (int32)||
|firstDeploy||false|boolean|false|
|firstDeployDate||false|integer (int64)||
|stageStartDate||false|integer (int64)||


