undo/scratch (scratch is in)
what does 'select that' do, and why isn't it selecting the whole word
look up selecting
finding - use `find it`, and `next one`
ordinal numbers/repeating

", ", comspace

**important words**
go, select, clear, copy, cut, paste,

`go address`

i added `drowse` as synonym for `talon sleep`

`slap` inserts new line down, i believe

`enter`


`junk`, 

(comma and | spamma | comspace): ", "

double paren : ()

Apps:
`launch [app]` - launches app
`focus [app]` - focuses an app
you can see the active apps by using `running list`






**undoing commands**
try `undo that`, or `scratch that`
command me.t

**tag**: user.tabs
-
`tab (open | new)`: app.tab_open()
`new tab`
tab (last | previous | left): app.tab_previous()
tab (next | right): app.tab_next()
tab close: user.tab_close_wrapper()
close tab
tab (reopen|restore): app.tab_reopen()
go tab <number>: user.tab_jump(number)
go tab final: user.tab_final()
tab duplicate: user.tab_duplicate()



**Browser**
tag: browser
-
address bar | go address | go url: browser.focus_address()
address copy | url copy | copy address | copy url:
    browser.focus_address()
    sleep(50ms)
    edit.copy()
go home: browser.go_home()
[go] forward: browser.go_forward()
go (back | backward): browser.go_back()
go to {user.website}: browser.go(website)
go private: browser.open_private_window()

bookmark it: browser.bookmark()
bookmark tabs: browser.bookmark_tabs()
(refresh | reload) it: browser.reload()
(refresh | reload) it hard: browser.reload_hard()

bookmark show: browser.bookmarks()
bookmark bar [show]: browser.bookmarks_bar()
downloads show: browser.show_downloads()
extensions show: browser.show_extensions()
history show: browser.show_history()
cache show: browser.show_clear_cache()



**rango**
There are two modes: direct and explicit clicking. To switch between them 
use the command rango direct or rango explicit.

**Direct Clicking**
just say the word
Examples
a: Clicks on link with the hint a
gh: Clicks on link with the hint gh
abc: Enters the characters abc
press a: Enters the character a
Explicit Clicking
With explicit clicking you have to precede every hint with the word click. This mode prevents any misclicks at the expense of being a bit more tedious.

Other Commands
hover <hint>: It hovers over the element. After 10 seconds the element will be automatically unhovered.
hover fix <hint>: It hovers over the element. The element will not be automatically unhovered.
dismiss: It clears any previously hovered element.
show <hint>: It shows the url address.
copy link <hint>: It copies the url address to the clipboard.
blank <hint>: It opens the link in a new tab.
hints toggle: It shows and hides the hints.



**Some other commands**
there's scroll down (standard.talon). is there page down?

page down? (in code/keys.py) - alternate keys is there as well

end
enter
escape (also, "leave")
home
insert
pagedown (also, "page down", "flow down", "roll down")
pageup (also, "page up", "flow up", "roll up")
space (also, "ace")
tab

Also, 
"delete" == "backspace",
'junk' == 'backspace',
"forward delete" == "delete",



**text**
I think the `ship` commande makes things capitalized. so `ship air` will make an `A`

find it:
    edit.find()

next one:
    edit.find_next()

go word left, go word right
go left, right, up, down
go line start, line end,
go way right, way left, way down, way up
go bottom, go top
go page down, go page up

# selecting
select this
select line, all, left, right, up, down
select word, word left, word right, 
select way left, way right, way up, way down

# editing
indent more
indend less | out dent

# deleting
clear line
clear left, right, up, down
clear word, word left, word right,
clear way left, way right, way up, way down, all

**copy commands**
copy all, word, work left, word right, line

**cut commands**
cut all, word, word left, word right, line   


**mouse/controls**
how to click - in rango it's `click [tag]`
in otherwise, it's `touch` for left click, `righty` for right click . adding in (`right click` for `righty` as)
`dubclick` for double clicking. all of this is in `mouse.talon`
to press a set of keys (or one key) use `press` 

down arrow?


there's `left drag | drag` and `right drag | righty drag` as well,
and `end drag| drag end` .


`misc/formatters.talon`
#provide both anchored and unachored commands via 'over'
phrase <user.text>$: user.insert_formatted(text, "NOOP")
phrase <user.text> over: user.insert_formatted(text, "NOOP")
{user.prose_formatter} <user.prose>$: user.insert_formatted(prose, prose_formatter)
{user.prose_formatter} <user.prose> over: user.insert_formatted(prose, prose_formatter)
<user.format_text>+$: user.insert_many(format_text_list)
<user.format_text>+ over: user.insert_many(format_text_list)
<user.formatters> that: user.formatters_reformat_selection(user.formatters)
word <user.word>: user.insert_formatted(user.word, "NOOP")
recent list: user.toggle_phrase_history()
recent close: user.phrase_history_hide()
recent repeat <number_small>: insert(user.get_recent_phrase(number_small))
recent copy <number_small>: clip.set_text(user.get_recent_phrase(number_small))
select that: user.select_last_phrase()
before that: user.before_last_phrase()
nope that | scratch that: user.clear_last_phrase()
nope that was <user.formatters>: user.formatters_reformat_last(formatters)




misheard words - `down` it hears as `dot`, `undo` as `end`
insead of `undo`, we should use



**vscode**
`toggle comment`
`indent more|less`
`show settings`
look more in vscode.talon
`please` - shows commands?



**cursorless**

**slack**
go search, or go findx  


chrome/email