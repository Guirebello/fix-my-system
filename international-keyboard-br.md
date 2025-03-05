# How to use an US international Keyboard for typing in Portuguese

Keyboard layout --> *us*
Variant: 
- *intl* (no altgr keys)
- *altgr-intl* (with altgr keys)
## Hyprland
The keyboard Layout you gotta use is:
```
input{
	kb_layout = us
	kb_variant = intl
	
#rest of your config ...
}
```


This solves the problem partially, if you want to use the (' + c) combination to generate ç its not gonna work, its gonna generate ć. What works is (right alt + ,).
	To solve this problem go to --> [[solving-cedilla-international-keyboard]]
