class Node:
    def __init__ (self,val):
        self.val=val
        self.next=None 
class Stack:
    def __init__ (self):
        self.head=Node("head")
        self.size=0
        
    def print(self):
        c=self.head.next
        o=""
        while c:
            o+=str(c.val)+" "
            c=c.next
        return o
    def getsize(self):
        return self.size
    def empty(self):
        return self.size==0 
    def peek(self):
        if self.empty():
            return "empty"
        return self.head.next.val
    def push(self,val):
        node=Node(val)
        node.next=self.head.next
        self.head.next=node
        self.size+=1 
    def pop(self):
        if self.empty():
            return "empty"
        r=self.head.next
        self.head.next=self.head.next.next
        self.size-=1 
        return r.val 
if __name__ =="__main__":
    stack=Stack()
    stack.push(12)
    stack.push(13)
    stack.push(14)
    stack.push(15)
    print(stack.print())
    print(stack.pop())
    print(stack.print())
    print(stack.peek())
