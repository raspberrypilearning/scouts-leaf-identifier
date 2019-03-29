```
when green flag clicked
ask [Is it a Is it a single leaf on it's own?] and wait
if <(answer) = [yes]> then
broadcast (hide compound v)
else
broadcast (hide simple v)
end 
```

```
when I receive [hide compound v]
ask [Does it have lobes sticking out?] and wait
if <> then
else
end 

broadcast (hide no lobes v)

<(answer) = [yes]>

broadcast (hide lobes v)
```

```
if <> then
else
end 

<(answer) = [yes]>

ask [Do the leaves spread from a point] and wait

when I receive [hide simple v]

broadcast [hide spread v]

broadcast [hide no spread v]
```

```
when I receive [hide no lobes v]
ask [Do the lobes spread from one point] and wait

broadcast [hide lobes line]

broadcast [hide lobes point]
```


```
when I receive [hide lobes v]

when I receive [hide spread v]

broadcast (hide round v)

broadcast (hide thin v)
```