# 功能实现

1. 在 `TaskControlBlock` 中添加系统调用数统计数组和任务的起始、现在时间
2. 在 `TASK_MANAGER` 初始化时，将任务起始时间利用 `get_time_ms()` 获取
3. 在任务切换前，更新任务的现在时间；在 `syscall()` 分发系统调用前，更新系统调用统计数组
4. `sys_task_info` 获取 `TaskControlBlock` 中相关信息，拷贝到 `TaskInfo` 指针中

# 问答题
