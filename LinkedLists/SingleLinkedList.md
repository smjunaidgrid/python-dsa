## Finding ref in LL 

#### Finding ref to the last node in the list

```
p = self.start
while p.link is not None:
    p= p.link
```

#### Finding ref to second last node 
```
p = self.start 
while p.link.link is not None:
    p = p.link
```

#### Finding ref to a node with particular info 
```
p = self.start 
while p is not None:
    if p.info == x:
        break
    p = p.link
```
#### Finding ref to predecessor of the node with particular info 

```
p = self.start 
while p.link is not None:
    if p.link.info == x:
        break 
    p = p.link
```

#### Finding the ref of the node at a particular position 

```
p = self.start 
i = 1 
while i < k and p is not None:
    p = p.link 
    i+=1
```

## Insertion in single LL
#### Inserting at the beginning of the list
```
temp.link = self.start 
self.start = temp 
```

#### Inserting in an empty List 
```
self.start = temp

```

#### Inserting at the end of list
```
p = self.start 
while p.link is not None:
    p = p.link
p.link = temp
```

#### Insertion between the nodes
```
temp.link = p.link 
p.link = temp
```

#### Insertion after node 
```
p = self.start 
while p is not None:
    if p.info == x:
        break
    p = p.link

```

#### Insertion before the node
```
p = self.start 
while p.link is not None:
    if p.link.info == x:
        break 
    p = p.link
```

#### Insert at a given position 
```
p = self.start 
while i<k-1 and p is not None:
    p = p.link
    i+=1
```

