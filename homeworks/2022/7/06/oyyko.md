分离的空闲链表：维护多个空闲链表，其中每个链表中的块有大致相等的大小。

例如按照2的幂来划分块大小。

分配器维护一个空闲链表数组，每一个大小类一个空闲链表。

搜索的时候从对应的空闲链表开始搜索，如果找不到合适的块就搜索下一个链表。