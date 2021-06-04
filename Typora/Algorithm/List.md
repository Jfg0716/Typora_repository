#### 1、判断给定的链表中是否有环。如果有环则返回true，否则返回false。

```java
//定义两个指针(fast、slow),fast每次走两步，slow每次走一步，若他们相遇则存在环
public boolean hasCycle(ListNode head) {
    if(head == null) return false;
    //定义fast和slow，起始指向头节点
    ListNode fast = head;
    ListNode slow = head;
    while(fast != null && fast.next != null){
        fast = fast.next.next;
        slow = slow.next;
        if(slow == fast) return true;
    }
    return false;
}
```

