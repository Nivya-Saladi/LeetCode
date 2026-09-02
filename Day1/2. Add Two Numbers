# Definition for singly-linked list.
# class ListNode:
#     def __init__(self, val=0, next=None):
#         self.val = val
#         self.next = next
class Solution:
    def addTwoNumbers(self, l1: Optional[ListNode], l2: Optional[ListNode]) -> Optional[ListNode]:
        temp = ListNode(0)
        current = temp
        carry = 0

        while l1 or l2:
            a = l1.val if l1 else 0
            b = l2.val if l2 else 0

            total = a+b+carry
            
            current.next = ListNode(total%10)
            carry = total // 10

            current = current.next
            if l1:
                l1 = l1.next
            if l2:
                l2 = l2.next
        if carry:
            current.next = ListNode(carry)
        return temp.next

        
