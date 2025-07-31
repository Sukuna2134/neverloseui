```Library
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/Sukuna2134/neverloseui/refs/heads/main/neverlose%20lib"))()
```

```Window
local Window = Library:Window({
    text = "Window"
})
```

```TabSection
local TabSection = Window:TabSection({
    text = "TabSection"
})
```

```Tab
local Tab = TabSection:Tab({
    text = "Tab",
    icon = "rbxassetid://7999345313",
})
```

```Section
local Section = Tab:Section({
    text = "Section"
})
```

```Button
Section:Button({
    text = "Button",
    callback = function()
        print("Clicked button")
    end,
})
```

```Toggle
Section:Toggle({
    text = "Toggle",
    state = false, -- Default boolean
    callback = function(boolean)
        print("Toggle current: ",boolean)
    end
})
```

```Slider
Section:Slider({
    text = "Slider",
    min = 10,
    max = 100,
    -- [[Float = 0,]] Idk what it does
    callback = function(number)
        print(number)
    end
})
```

```Dropdown
Section:Dropdown({
    text = "Dropdown",
    list = {"Apple", "Banana","Coconut"},
    default = "Apple",
    callback = function(String)
        print(String)
    end
})
```

```Textbox
Section:Textbox({
    text = "Textbox",
    value = "Default",
    callback = function(String)
        print(String)
    end
})
```

```Colorpicker
Section:Colorpicker({
    text = "Colorpicker",
    color = Color3.new(1,1,1),
    callback = function(HSV)
        print(HSV)
    end
})
```

```Keybind
Section:Keybind({
    text = "Keybind",
    default = Enum.KeyCode.Z,
    callback = function(defaultBind)
        print("Triggered keybind")
        print(defaultBind)
    end
})
```
