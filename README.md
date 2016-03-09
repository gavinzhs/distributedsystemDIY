# distributedsystemDIY
##一个最简单的分布式系统
1. request -> balance -> worker
	1. balance register all workers
	1. 请求方访问balance server
	1. balance server根据根据算法(任务最少者)选择worker处理request
	1. worker处理结束后，通知balance任务完成，并把结果交还给reques
