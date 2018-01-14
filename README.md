Tearing your hair out getting ready for a PCI audit?  Trying to meet yet another requirement with minimal code changes?

Mask the PAN during data entry with a custom font and css only.  No javascript needed.


## How to Use
### Reveal on focus
```
input.secretfy {
    font-family: 'secretfy';
}
input.secretfy:focus {
    font: initial;
}
```

### Reveal on hover also
```
input.secretfy {
    font-family: 'secretfy';
}
input.secretfy:hover, input.secretfy:focus {
    font: initial;
}
```

### April Fools
```
input.secretfy {
    font-family: 'secretfy';
}
```

#

## Disclaimer
This is provided as is.  Author is not responsible if you fail a PCI audit from using any software or advice provided.

#

## Alternatives if you do not want to use secretfy
### Use type="password"
Use javascript to change the input from text to password when the input loses focus.

Cons:
* Javascript needed
* Browsers will prompt to save the password field

### Use another variable
There are few variants of this approach.  It involves using a javascript variable or hidden input to keep the real user inputted text.  The form field value visible in the UI is redacted.

Cons:
* Even more Javascript
