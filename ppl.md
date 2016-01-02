# PPL #



`ppl [-ac] [cmd] [@alias] [name] [number] `

  * Main commands: add delete edit help list read
  * Recipients: prepend @ to aliases. phonenumbers should be +0-9, >3digits

```
> ppl add test 0104669090 # adds an entry for person named test
> ppl @test # print details of person @test
> ppl delete @test # deletes it again
```


---

# Subcommands #


### ppl add ###
`ppl add (name) (number) `
> add person info.
> prompts for name or number if needed.

### ppl config ###
`ppl config `
> open $EDITOR with ~/.thone/ppl.rc
> restart Thone to have changes take effect

### ppl delete ###
`ppl delete (@alias|number|name|id) `
> deletes ppl from ppl.cache and from dbus.

### ppl edit ###
`ppl edit (@alias|number|name|id) `
> prompts to change the number or name.
> saves changes to dbus

### ppl help ###
`ppl help`
> some help

### ppl list ###
`ppl list `
> displays all ppl, short form

### ppl read ###
`ppl [read] (@alias|number|name|id) `
> default command
> displays person info, long form

### ppl touch ###
`ppl touch (@alias|number|name|id) uts`
> renames the ppl file to match uts timestamp
> of the last time this person was contacted.
> only usefull for future apps.

### ppl update ###
`ppl update`
> sync the local ppl.cache with dbus storage

### ppl -ac ###
`ppl -ac [arguments]`
> performs autocomplete on last argument