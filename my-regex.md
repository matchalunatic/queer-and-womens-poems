# Regex to keep formatting in poems from raw text to md (for vim)

## Honor spacing

```
:'<,'>s/  \+/\=repeat("&nbsp;",strlen(submatch(0)))
```

## Line breaks

```
:'<,'>s@$@  @g
```
