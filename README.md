## Loadstring
```lua
local developer = "BOXLEGENDARY"
local branch = "main"

local function webImport(file)
    return loadstring(game:HttpGetAsync(("https://raw.githubusercontent.com/%s/Hydroxide/%s/%s.lua"):format(developer, branch, file)), file .. '.lua')()
end

webImport("init")
webImport("ui/main")
```
