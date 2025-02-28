## Script
```lua
local owner = "astroctrl"
local branch = "revision"

local function webImport(file)
    return loadstring(game:HttpGetAsync(("https://raw.githubusercontent.com/%s/Hydroxide/%s/%s.lua"):format(owner, branch, file)), file .. '.lua')()
end

webImport("init")
webImport("ui/main")
```

# Hydroxide
<i>This version of hydroxide was modified to use trampolineMetatableHook to stay undetected</i>