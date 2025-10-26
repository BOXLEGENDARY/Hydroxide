## Loadstring
```lua
local user = "BOXLEGENDARY"
local branch = "main"

local function webImport(file)
    return loadstring(game:HttpGetAsync(("https://raw.githubusercontent.com/%s/Hydroxide/%s/%s.lua"):format(user, branch, file)), file .. '.lua')()
end

webImport("init")
webImport("ui/main")
```
