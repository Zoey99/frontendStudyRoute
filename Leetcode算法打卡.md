## Leetcode算法打卡

#### 5.11

- [x] 21.合并两个有序链表

  ```javascript
  var mergeTwoLists = function(l1, l2) {
      let curr=new ListNode();
      let head = curr;
      while(l1!== null && l2 !==null){
          if(l1.val<l2.val)
          {
              curr.next = l1;
              l1 = l1.next;
          }
          else
          {
              curr.next = l2;
              l2= l2.next
          }
          curr = curr.next;
      }
      if(l1!==null){
          curr.next = l1;
      }
      if(l2!==null){
          curr.next = l2;
      }
      return head.next;
  };
  ```

  

- [ ] 148.排序链表

- [ ] 25.K个一组翻转链表

#### 5.12

- [ ] 13.罗马数字转整数
- [ ] 12.整数转罗马数字
- [ ] 32.最长有效括号