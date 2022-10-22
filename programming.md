
# programming.md

Some notes about programming the HP-42s and its descendants.

## Labels

### Global Labels

`LBL "TEST"`

### Local Labels

`LBL 00` → `LBL 99`

`LBL A`→ `LBL J`
`LBL a`→ `LBL e`


## Registers


## Variables


## Looping with `ISG` and `DSE`

```sql
; sss.eeeii or sss.eee (start s, end e, increment i)
1.05203
STO "COUNT"
LBL 01
; ...
ISG "COUNT"
GTO 01 ; while COUNT is < 52
BEEP
```

`ISG _var_` increment and skip if counter > end

`DSE _var_` decrement and skip if counter ≤ end


## Command List

### ABS ← `x`

Replaces `x` with `|x|`.

### ...

### PIXEL ← `x` `y`

Turns on pixel at `(x, y)`.

