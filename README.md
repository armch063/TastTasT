local function loading()
	local Loading = Instance.new("ScreenGui")
	local Blur = Instance.new("Frame")
	local Main = Instance.new("Frame")
	local UICorner = Instance.new("UICorner")
	local Logo = Instance.new("ImageLabel")
	local UICorner_2 = Instance.new("UICorner")
	local Load = Instance.new("Frame")
	local UICorner_3 = Instance.new("UICorner")
	local Bar = Instance.new("Frame")
	local UICorner_4 = Instance.new("UICorner")
	local BAR1 = Instance.new("Frame")
	local UICorner_5 = Instance.new("UICorner")
	local TextLabel = Instance.new("TextLabel")
	local Top = Instance.new("Frame")
	local UICorner_6 = Instance.new("UICorner")
	local TextLabel_2 = Instance.new("TextLabel")
	local TextLabel_3 = Instance.new("TextLabel")

	--Properties:

	Loading.Name = "Loading"
	Loading.Parent = game.CoreGui
	Loading.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

	Blur.Name = "Blur"
	Blur.Parent = Loading
	Blur.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
	Blur.BackgroundTransparency = 1
	Blur.Size = UDim2.new(1, 0, 1, 0)

	Main.Name = "Main"
	Main.Parent = Blur
	Main.AnchorPoint = Vector2.new(0.5, 0.5)
	Main.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
	Main.ClipsDescendants = true
	Main.Position = UDim2.new(0.5, 0, 0.499241263, 0)
	Main.Size = UDim2.new(0, 500, 0, 300)

	UICorner.Parent = Main

	Logo.Name = "Logo"
	Logo.Parent = Main
	Logo.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
	Logo.Position = UDim2.new(0.400000006, 0, 0.163333327, 0)
	Logo.Size = UDim2.new(0, 100, 0, 100)
	Logo.Image = "http://www.roblox.com/asset/?id=9779739843"

	UICorner_2.CornerRadius = UDim.new(0, 100)
	UICorner_2.Parent = Logo

	Load.Name = "Load"
	Load.Parent = Main
	Load.BackgroundColor3 = Color3.fromRGB(35, 35, 35)
	Load.Position = UDim2.new(0, 15, 0, 170)
	Load.Size = UDim2.new(0, 470, 0, 115)

	UICorner_3.Parent = Load

	Bar.Name = "Bar"
	Bar.Parent = Load
	Bar.BackgroundColor3 = Color3.fromRGB(25, 25, 25)
	Bar.Position = UDim2.new(0, 15, 0, 80)
	Bar.Size = UDim2.new(0, 440, 0, 15)

	UICorner_4.CornerRadius = UDim.new(0, 5)
	UICorner_4.Parent = Bar

	BAR1.Name = "BAR1"
	BAR1.Parent = Bar
	BAR1.BackgroundColor3 = Color3.fromRGB(255,199,41)
	BAR1.Size = UDim2.new(0, 0, 0, 15)

	UICorner_5.CornerRadius = UDim.new(0, 5)
	UICorner_5.Parent = BAR1

	TextLabel.Parent = Load
	TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	TextLabel.BackgroundTransparency = 1.000
	TextLabel.Position = UDim2.new(0.0319148935, 0, 0.173913032, 0)
	TextLabel.Size = UDim2.new(0, 440, 0, 25)
	TextLabel.Font = Enum.Font.GothamSemibold
	TextLabel.Text = "Loading"
	TextLabel.TextColor3 = Color3.fromRGB(225, 225, 225)
	TextLabel.TextSize = 16.000
	spawn(function()
		for i = 1,5 do 
			wait(0.5)
			TextLabel.Text = "Loading."
			wait(0.5) 
			TextLabel.Text = "Loading.."
			wait(0.5)
			TextLabel.Text = "Loading..."
		end
	end)

	Top.Name = "Top"
	Top.Parent = Main
	Top.BackgroundColor3 = Color3.fromRGB(35, 35, 35)
	Top.Size = UDim2.new(0, 500, 0, 30)

	UICorner_6.Parent = Top

	TextLabel_2.Parent = Top
	TextLabel_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	TextLabel_2.BackgroundTransparency = 1.000
	TextLabel_2.Position = UDim2.new(0.0299999993, 0, 0, 0)
	TextLabel_2.Size = UDim2.new(0, 61, 0, 30)
	TextLabel_2.Font = Enum.Font.GothamSemibold
	TextLabel_2.Text = "  SHADOW"
	TextLabel_2.TextColor3 = Color3.fromRGB(225, 225, 225)
	TextLabel_2.TextSize = 17.000

	TextLabel_3.Parent = Top
	TextLabel_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
	TextLabel_3.BackgroundTransparency = 1.000
	TextLabel_3.Position = UDim2.new(0.151999995, 0, 0, 0)
	TextLabel_3.Size = UDim2.new(0, 61, 0, 30)
	TextLabel_3.Font = Enum.Font.GothamSemibold
	TextLabel_3.Text = "   HUB"
	TextLabel_3.TextColor3 = Color3.fromRGB(255,199,41)
	TextLabel_3.TextSize = 17.000
	TextLabel_3.TextXAlignment = Enum.TextXAlignment.Left
	
	BAR1:TweenSize(UDim2.new(0,440,0,15),"Out","Linear",5,true)
	wait(5)
    Main:TweenSize(UDim2.new(0,0,0,0),"Out","Quad",0.4,true)
    wait(0.6)
	
	do 
		local Load = game.CoreGui:FindFirstChild("Loading")
		if Load then
			Load:Destroy()
		end
	end
end
loading()

local ScreenGui = Instance.new("ScreenGui")
local ImageButton = Instance.new("ImageButton")

ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

ImageButton.Parent = ScreenGui
ImageButton.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
ImageButton.BorderSizePixel = 0
ImageButton.Position = UDim2.new(0.120833337, 0, 0.0952890813, 0)
ImageButton.Size = UDim2.new(0, 50, 0, 50)
ImageButton.Image = "http://www.roblox.com/asset/?id=9779739843"
ImageButton.MouseButton1Down:connect(function()
    game:GetService("VirtualInputManager"):SendKeyEvent(true,305,false,game)
    game:GetService("VirtualInputManager"):SendKeyEvent(false,305,false,game)
end)

_G.FastAttack = true
_G.AutoHaki = true
_G.WalkOnWater = true
Magnet = true

do local GUI = game.CoreGui:FindFirstChild("SHADOWHUB");if GUI then GUI:Destroy();end;if _G.Color == nil then
        _G.Color = Color3.fromRGB(255,199,41)
    end
end

    local UserInputService = game:GetService("UserInputService")
    local TweenService = game:GetService("TweenService")
    
    local function MakeDraggable(topbarobject, object)
    local Dragging = nil
    local DragInput = nil
    local DragStart = nil
    local StartPosition = nil
    
    local function Update(input)
     local Delta = input.Position - DragStart
     local pos = UDim2.new(StartPosition.X.Scale, StartPosition.X.Offset + Delta.X, StartPosition.Y.Scale, StartPosition.Y.Offset + Delta.Y)
     local Tween = TweenService:Create(object, TweenInfo.new(0.15), {Position = pos})
     Tween:Play()
    end
    
    topbarobject.InputBegan:Connect(
     function(input)
         if input.UserInputType == Enum.UserInputType.MouseButton1 or input.UserInputType == Enum.UserInputType.Touch then
             Dragging = true
             DragStart = input.Position
             StartPosition = object.Position
    
             input.Changed:Connect(
                 function()
                     if input.UserInputState == Enum.UserInputState.End then
                         Dragging = false
                     end
                 end
             )
         end
     end
    )
    
    topbarobject.InputChanged:Connect(
     function(input)
         if
             input.UserInputType == Enum.UserInputType.MouseMovement or
             input.UserInputType == Enum.UserInputType.Touch
         then
             DragInput = input
         end
     end
    )
    
    UserInputService.InputChanged:Connect(
     function(input)
         if input == DragInput and Dragging then
             Update(input)
         end
     end
    )
    end
    
    local Update = {}
    
    function Update:Window(text,logo,keybind)
    local uihide = false
    local abc = false
    local logo = logo or 0
    local currentpage = ""
    local keybind = keybind or Enum.KeyCode.RightControl
    local yoo = string.gsub(tostring(keybind),"Enum.KeyCode.","")
    
    local SHADOWHUB = Instance.new("ScreenGui")
    SHADOWHUB.Name = "SHADOWHUB"
    SHADOWHUB.Parent = game.CoreGui
    SHADOWHUB.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
    
    local Main = Instance.new("Frame")
    Main.Name = "Main"
    Main.Parent = SHADOWHUB
    Main.ClipsDescendants = true
    Main.AnchorPoint = Vector2.new(0.5,0.5)
    Main.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
    Main.Position = UDim2.new(0.5, 0, 0.5, 0)
    Main.Size = UDim2.new(0, 0, 0, 0)
    
    Main:TweenSize(UDim2.new(0, 656, 0, 400),"Out","Quad",0.4,true)
    
    local MCNR = Instance.new("UICorner")
    MCNR.Name = "MCNR"
    MCNR.Parent = Main
    
    local Top = Instance.new("Frame")
    Top.Name = "Top"
    Top.Parent = Main
    Top.BackgroundColor3 = Color3.fromRGB(35, 35, 35)
    Top.Size = UDim2.new(0, 656, 0, 27)
    
    local TCNR = Instance.new("UICorner")
    TCNR.Name = "TCNR"
    TCNR.Parent = Top
    
    local Logo = Instance.new("ImageLabel")
    Logo.Name = "Logo"
    Logo.Parent = Top
    Logo.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    Logo.BackgroundTransparency = 1.000
    Logo.Position = UDim2.new(0, 10, 0, 1)
    Logo.Size = UDim2.new(0, 25, 0, 25)
    Logo.Image = "http://www.roblox.com/asset/?id=9779739843"..tostring(logo)
    
    local Name = Instance.new("TextLabel")
    Name.Name = "Name"
    Name.Parent = Top
    Name.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    Name.BackgroundTransparency = 1.000
    Name.Position = UDim2.new(0.0609756112, 0, 0, 0)
    Name.Size = UDim2.new(0, 61, 0, 27)
    Name.Font = Enum.Font.GothamSemibold
    Name.Text = text
    Name.TextColor3 = Color3.fromRGB(255, 255, 255)
    Name.TextSize = 17.000
    
    local Hub = Instance.new("TextLabel")
    Hub.Name = "Hub"
    Hub.Parent = Top
    Hub.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    Hub.BackgroundTransparency = 1.000
    Hub.Position = UDim2.new(0, 110, 0, 0)
    Hub.Size = UDim2.new(0, 81, 0, 27)
    Hub.Font = Enum.Font.GothamSemibold
    Hub.Text = "   HUB"
    Hub.TextColor3 = _G.Color
    Hub.TextSize = 17.000
    Hub.TextXAlignment = Enum.TextXAlignment.Left
    
    local BindButton = Instance.new("TextButton")
    BindButton.Name = "BindButton"
    BindButton.Parent = Top
    BindButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    BindButton.BackgroundTransparency = 1.000
    BindButton.Position = UDim2.new(0.847561002, 0, 0, 0)
    BindButton.Size = UDim2.new(0, 100, 0, 27)
    BindButton.Font = Enum.Font.GothamSemibold
    BindButton.Text = "[ "..string.gsub(tostring(keybind),"Enum.KeyCode.","").." ]"
    BindButton.TextColor3 = Color3.fromRGB(100, 100, 100)
    BindButton.TextSize = 11.000
    
    BindButton.MouseButton1Click:Connect(function ()
     BindButton.Text = "[ ... ]"
     local inputwait = game:GetService("UserInputService").InputBegan:wait()
     local shiba = inputwait.KeyCode == Enum.KeyCode.Unknown and inputwait.UserInputType or inputwait.KeyCode
    
     if shiba.Name ~= "Focus" and shiba.Name ~= "MouseMovement" then
         BindButton.Text = "[ "..shiba.Name.." ]"
         yoo = shiba.Name
     end
    end)
    
    local Tab = Instance.new("Frame")
    Tab.Name = "Tab"
    Tab.Parent = Main
    Tab.BackgroundColor3 = Color3.fromRGB(35, 35, 35)
    Tab.Position = UDim2.new(0, 5, 0, 30)
    Tab.Size = UDim2.new(0, 150, 0, 365)
    
    local TCNR = Instance.new("UICorner")
    TCNR.Name = "TCNR"
    TCNR.Parent = Tab
    
    local ScrollTab = Instance.new("ScrollingFrame")
    ScrollTab.Name = "ScrollTab"
    ScrollTab.Parent = Tab
    ScrollTab.Active = true
    ScrollTab.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    ScrollTab.BackgroundTransparency = 1.000
    ScrollTab.Size = UDim2.new(0, 150, 0, 365)
    ScrollTab.CanvasSize = UDim2.new(0, 0, 0, 0)
    ScrollTab.ScrollBarThickness = 0
    
    local PLL = Instance.new("UIListLayout")
    PLL.Name = "PLL"
    PLL.Parent = ScrollTab
    PLL.SortOrder = Enum.SortOrder.LayoutOrder
    PLL.Padding = UDim.new(0, 15)
    
    local PPD = Instance.new("UIPadding")
    PPD.Name = "PPD"
    PPD.Parent = ScrollTab
    PPD.PaddingLeft = UDim.new(0, 10)
    PPD.PaddingTop = UDim.new(0, 10)
    
    local Page = Instance.new("Frame")
    Page.Name = "Page"
    Page.Parent = Main
    Page.BackgroundColor3 = Color3.fromRGB(35, 35, 35)
    Page.Position = UDim2.new(0.245426834, 0, 0.075000003, 0)
    Page.Size = UDim2.new(0, 490, 0, 365)
    
    local PCNR = Instance.new("UICorner")
    PCNR.Name = "PCNR"
    PCNR.Parent = Page
    
    local MainPage = Instance.new("Frame")
    MainPage.Name = "MainPage"
    MainPage.Parent = Page
    MainPage.ClipsDescendants = true
    MainPage.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    MainPage.BackgroundTransparency = 1.000
    MainPage.Size = UDim2.new(0, 490, 0, 365)
    
    local PageList = Instance.new("Folder")
    PageList.Name = "PageList"
    PageList.Parent = MainPage
    
    local UIPageLayout = Instance.new("UIPageLayout")
    
    UIPageLayout.Parent = PageList
    UIPageLayout.SortOrder = Enum.SortOrder.LayoutOrder
    UIPageLayout.EasingDirection = Enum.EasingDirection.InOut
    UIPageLayout.EasingStyle = Enum.EasingStyle.Quad
    UIPageLayout.FillDirection = Enum.FillDirection.Vertical
    UIPageLayout.Padding = UDim.new(0, 15)
    UIPageLayout.TweenTime = 0.400
    UIPageLayout.GamepadInputEnabled = false
    UIPageLayout.ScrollWheelInputEnabled = false
    UIPageLayout.TouchInputEnabled = false
    
    MakeDraggable(Top,Main)
    
    UserInputService.InputBegan:Connect(function(input)
     if input.KeyCode == Enum.KeyCode[yoo] then
         if uihide == false then
             uihide = true
             Main:TweenSize(UDim2.new(0, 0, 0, 0),"In","Quad",0.4,true)
         else
             uihide = false
             Main:TweenSize(UDim2.new(0, 656, 0, 400),"Out","Quad",0.4,true)
         end
     end
    end)
    
    local uitab = {}
    
    function uitab:Tab(text)
     local TabButton = Instance.new("TextButton")
     TabButton.Parent = ScrollTab
     TabButton.Name = text.."Server"
     TabButton.Text = text
     TabButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
     TabButton.BackgroundTransparency = 1.000
     TabButton.Size = UDim2.new(0, 130, 0, 23)
     TabButton.Font = Enum.Font.GothamSemibold
     TabButton.TextColor3 = Color3.fromRGB(255, 255, 255)
     TabButton.TextSize = 15.000
     TabButton.TextTransparency = 0.500
    
     local MainFramePage = Instance.new("ScrollingFrame")
     MainFramePage.Name = text.."_Page"
     MainFramePage.Parent = PageList
     MainFramePage.Active = true
     MainFramePage.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
     MainFramePage.BackgroundTransparency = 1.000
     MainFramePage.BorderSizePixel = 0
     MainFramePage.Size = UDim2.new(0, 490, 0, 365)
     MainFramePage.CanvasSize = UDim2.new(0, 0, 0, 0)
     MainFramePage.ScrollBarThickness = 0
     
     local UIPadding = Instance.new("UIPadding")
     local UIListLayout = Instance.new("UIListLayout")
     
     UIPadding.Parent = MainFramePage
     UIPadding.PaddingLeft = UDim.new(0, 10)
     UIPadding.PaddingTop = UDim.new(0, 10)
    
     UIListLayout.Padding = UDim.new(0,15)
     UIListLayout.Parent = MainFramePage
     UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder
     
     TabButton.MouseButton1Click:Connect(function()
         for i,v in next, ScrollTab:GetChildren() do
             if v:IsA("TextButton") then
                 TweenService:Create(
                     v,
                     TweenInfo.new(0.3,Enum.EasingStyle.Quad,Enum.EasingDirection.Out),
                     {TextTransparency = 0.5}
                 ):Play()
             end
             TweenService:Create(
                 TabButton,
                 TweenInfo.new(0.3,Enum.EasingStyle.Quad,Enum.EasingDirection.Out),
                 {TextTransparency = 0}
             ):Play()
         end
         for i,v in next, PageList:GetChildren() do
             currentpage = string.gsub(TabButton.Name,"Server","").."_Page"
             if v.Name == currentpage then
                 UIPageLayout:JumpTo(v)
             end
         end
     end)
    
     if abc == false then
         for i,v in next, ScrollTab:GetChildren() do
             if v:IsA("TextButton") then
                 TweenService:Create(
                     v,
                     TweenInfo.new(0.3,Enum.EasingStyle.Quad,Enum.EasingDirection.Out),
                     {TextTransparency = 0.5}
                 ):Play()
             end
             TweenService:Create(
                 TabButton,
                 TweenInfo.new(0.3,Enum.EasingStyle.Quad,Enum.EasingDirection.Out),
                 {TextTransparency = 0}
             ):Play()
         end
         UIPageLayout:JumpToIndex(1)
         abc = true
     end
     
     game:GetService("RunService").Stepped:Connect(function()
         pcall(function()
             MainFramePage.CanvasSize = UDim2.new(0,0,0,UIListLayout.AbsoluteContentSize.Y + 20)
             ScrollTab.CanvasSize = UDim2.new(0,0,0,PLL.AbsoluteContentSize.Y + 20)
         end)
     end)
     
     local main = {}
     function main:Button(text,callback)
         local Button = Instance.new("Frame")
         local UICorner = Instance.new("UICorner")
         local TextBtn = Instance.new("TextButton")
         local UICorner_2 = Instance.new("UICorner")
         local Black = Instance.new("Frame")
         local UICorner_3 = Instance.new("UICorner")
         
         Button.Name = "Button"
         Button.Parent = MainFramePage
         Button.BackgroundColor3 = _G.Color
         Button.Size = UDim2.new(0, 470, 0, 31)
         
         UICorner.CornerRadius = UDim.new(0, 5)
         UICorner.Parent = Button
         
         TextBtn.Name = "TextBtn"
         TextBtn.Parent = Button
         TextBtn.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
         TextBtn.Position = UDim2.new(0, 1, 0, 1)
         TextBtn.Size = UDim2.new(0, 468, 0, 29)
         TextBtn.AutoButtonColor = false
         TextBtn.Font = Enum.Font.GothamSemibold
         TextBtn.Text = text
         TextBtn.TextColor3 = Color3.fromRGB(225, 225, 225)
         TextBtn.TextSize = 15.000
         
         UICorner_2.CornerRadius = UDim.new(0, 5)
         UICorner_2.Parent = TextBtn
         
         Black.Name = "Black"
         Black.Parent = Button
         Black.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
         Black.BackgroundTransparency = 1.000
         Black.BorderSizePixel = 0
         Black.Position = UDim2.new(0, 1, 0, 1)
         Black.Size = UDim2.new(0, 468, 0, 29)
         
         UICorner_3.CornerRadius = UDim.new(0, 5)
         UICorner_3.Parent = Black
    
         TextBtn.MouseEnter:Connect(function()
             TweenService:Create(
                 Black,
                 TweenInfo.new(0.4,Enum.EasingStyle.Quad,Enum.EasingDirection.Out),
                 {BackgroundTransparency = 0.7}
             ):Play()
         end)
         TextBtn.MouseLeave:Connect(function()
             TweenService:Create(
                 Black,
                 TweenInfo.new(0.4,Enum.EasingStyle.Quad,Enum.EasingDirection.Out),
                 {BackgroundTransparency = 1}
             ):Play()
         end)
         TextBtn.MouseButton1Click:Connect(function()
             TextBtn.TextSize = 0
             TweenService:Create(
                 TextBtn,
                 TweenInfo.new(0.4,Enum.EasingStyle.Quad,Enum.EasingDirection.Out),
                 {TextSize = 15}
             ):Play()
             callback()
         end)
     end
     function main:Toggle(text,config,callback)
         config = config or false
         local toggled = config
         local Toggle = Instance.new("Frame")
         local UICorner = Instance.new("UICorner")
         local Button = Instance.new("TextButton")
         local UICorner_2 = Instance.new("UICorner")
         local Label = Instance.new("TextLabel")
         local ToggleImage = Instance.new("Frame")
         local UICorner_3 = Instance.new("UICorner")
         local Circle = Instance.new("Frame")
         local UICorner_4 = Instance.new("UICorner")
    
         Toggle.Name = "Toggle"
         Toggle.Parent = MainFramePage
         Toggle.BackgroundColor3 = _G.Color
         Toggle.Size = UDim2.new(0, 470, 0, 31)
    
         UICorner.CornerRadius = UDim.new(0, 5)
         UICorner.Parent = Toggle
    
         Button.Name = "Button"
         Button.Parent = Toggle
         Button.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
         Button.Position = UDim2.new(0, 1, 0, 1)
         Button.Size = UDim2.new(0, 468, 0, 29)
         Button.AutoButtonColor = false
         Button.Font = Enum.Font.SourceSans
         Button.Text = ""
         Button.TextColor3 = Color3.fromRGB(0, 0, 0)
         Button.TextSize = 11.000
    
         UICorner_2.CornerRadius = UDim.new(0, 5)
         UICorner_2.Parent = Button
    
         Label.Name = "Label"
         Label.Parent = Toggle
         Label.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
         Label.BackgroundTransparency = 1.000
         Label.Position = UDim2.new(0, 1, 0, 1)
         Label.Size = UDim2.new(0, 468, 0, 29)
         Label.Font = Enum.Font.GothamSemibold
         Label.Text = text
         Label.TextColor3 = Color3.fromRGB(255, 255, 255)
         Label.TextSize = 15.000
    
         ToggleImage.Name = "ToggleImage"
         ToggleImage.Parent = Toggle
         ToggleImage.BackgroundColor3 = Color3.fromRGB(225, 225, 225)
         ToggleImage.Position = UDim2.new(0, 415, 0, 5)
         ToggleImage.Size = UDim2.new(0, 45, 0, 20)
    
         UICorner_3.CornerRadius = UDim.new(0, 10)
         UICorner_3.Parent = ToggleImage
    
         Circle.Name = "Circle"
         Circle.Parent = ToggleImage
         Circle.BackgroundColor3 = Color3.fromRGB(227, 60, 60)
         Circle.Position = UDim2.new(0, 2, 0, 2)
         Circle.Size = UDim2.new(0, 16, 0, 16)
    
         UICorner_4.CornerRadius = UDim.new(0, 10)
         UICorner_4.Parent = Circle
    
         Button.MouseButton1Click:Connect(function()
             if toggled == false then
                 toggled = true
                 Circle:TweenPosition(UDim2.new(0,27,0,2),"Out","Sine",0.2,true)
                 TweenService:Create(
                     Circle,
                     TweenInfo.new(0.4,Enum.EasingStyle.Quad,Enum.EasingDirection.Out),
                     {BackgroundColor3 = _G.Color}
                 ):Play()
             else
                 toggled = false
                 Circle:TweenPosition(UDim2.new(0,2,0,2),"Out","Sine",0.2,true)
                 TweenService:Create(
                     Circle,
                     TweenInfo.new(0.4,Enum.EasingStyle.Quad,Enum.EasingDirection.Out),
                     {BackgroundColor3 = Color3.fromRGB(227, 60, 110)}
                 ):Play()
             end
             pcall(callback,toggled)
         end)
    
         if config == true then
             toggled = true
             Circle:TweenPosition(UDim2.new(0,27,0,2),"Out","Sine",0.4,true)
             TweenService:Create(
                 Circle,
                 TweenInfo.new(0.4,Enum.EasingStyle.Quad,Enum.EasingDirection.Out),
                 {BackgroundColor3 = _G.Color}
             ):Play()
             pcall(callback,toggled)
         end
     end
     function main:Dropdown(text,option,callback)
         local isdropping = false
         local Dropdown = Instance.new("Frame")
         local UICorner = Instance.new("UICorner")
         local DropTitle = Instance.new("TextLabel")
         local DropScroll = Instance.new("ScrollingFrame")
         local UIListLayout = Instance.new("UIListLayout")
         local UIPadding = Instance.new("UIPadding")
         local DropButton = Instance.new("TextButton")
         local DropImage = Instance.new("ImageLabel")
         
         Dropdown.Name = "Dropdown"
         Dropdown.Parent = MainFramePage
         Dropdown.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
         Dropdown.ClipsDescendants = true
         Dropdown.Size = UDim2.new(0, 470, 0, 31)
         
         UICorner.CornerRadius = UDim.new(0, 5)
         UICorner.Parent = Dropdown
         
         DropTitle.Name = "DropTitle"
         DropTitle.Parent = Dropdown
         DropTitle.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
         DropTitle.BackgroundTransparency = 1.000
         DropTitle.Size = UDim2.new(0, 470, 0, 31)
         DropTitle.Font = Enum.Font.GothamSemibold
         DropTitle.Text = text.. " : "
         DropTitle.TextColor3 = Color3.fromRGB(225, 225, 225)
         DropTitle.TextSize = 15.000
         
         DropScroll.Name = "DropScroll"
         DropScroll.Parent = DropTitle
         DropScroll.Active = true
         DropScroll.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
         DropScroll.BackgroundTransparency = 1.000
         DropScroll.BorderSizePixel = 0
         DropScroll.Position = UDim2.new(0, 0, 0, 31)
         DropScroll.Size = UDim2.new(0, 470, 0, 100)
         DropScroll.CanvasSize = UDim2.new(0, 0, 0, 0)
         DropScroll.ScrollBarThickness = 3
         
         UIListLayout.Parent = DropScroll
         UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder
         UIListLayout.Padding = UDim.new(0, 5)
         
         UIPadding.Parent = DropScroll
         UIPadding.PaddingLeft = UDim.new(0, 5)
         UIPadding.PaddingTop = UDim.new(0, 5)
         
         DropImage.Name = "DropImage"
         DropImage.Parent = Dropdown
         DropImage.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
         DropImage.BackgroundTransparency = 1.000
         DropImage.Position = UDim2.new(0, 445, 0, 6)
         DropImage.Rotation = 180.000
         DropImage.Size = UDim2.new(0, 20, 0, 20)
         DropImage.Image = "rbxassetid://6031090990"
         
         DropButton.Name = "DropButton"
         DropButton.Parent = Dropdown
         DropButton.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
         DropButton.BackgroundTransparency = 1.000
         DropButton.Size = UDim2.new(0, 470, 0, 31)
         DropButton.Font = Enum.Font.SourceSans
         DropButton.Text = ""
         DropButton.TextColor3 = Color3.fromRGB(0, 0, 0)
         DropButton.TextSize = 14.000
    
         for i,v in next,option do
             local Item = Instance.new("TextButton")
    
             Item.Name = "Item"
             Item.Parent = DropScroll
             Item.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
             Item.BackgroundTransparency = 1.000
             Item.Size = UDim2.new(0, 460, 0, 26)
             Item.Font = Enum.Font.GothamSemibold
             Item.Text = tostring(v)
             Item.TextColor3 = Color3.fromRGB(225, 225, 225)
             Item.TextSize = 13.000
             Item.TextTransparency = 0.500
    
             Item.MouseEnter:Connect(function()
                 TweenService:Create(
                     Item,
                     TweenInfo.new(0.3,Enum.EasingStyle.Quad,Enum.EasingDirection.Out),
                     {TextTransparency = 0}
                 ):Play()
             end)
    
             Item.MouseLeave:Connect(function()
                 TweenService:Create(
                     Item,
                     TweenInfo.new(0.3,Enum.EasingStyle.Quad,Enum.EasingDirection.Out),
                     {TextTransparency = 0.5}
                 ):Play()
             end)
    
             Item.MouseButton1Click:Connect(function()
                 isdropping = false
                 Dropdown:TweenSize(UDim2.new(0,470,0,31),"Out","Quad",0.3,true)
                 TweenService:Create(
                     DropImage,
                     TweenInfo.new(0.3,Enum.EasingStyle.Quad,Enum.EasingDirection.Out),
                     {Rotation = 180}
                 ):Play()
                 callback(Item.Text)
                 DropTitle.Text = text.." : "..Item.Text
             end)
         end
    
         DropScroll.CanvasSize = UDim2.new(0,0,0,UIListLayout.AbsoluteContentSize.Y + 10)
    
         DropButton.MouseButton1Click:Connect(function()
             if isdropping == false then
                 isdropping = true
                 Dropdown:TweenSize(UDim2.new(0,470,0,131),"Out","Quad",0.3,true)
                 TweenService:Create(
                     DropImage,
                     TweenInfo.new(0.3,Enum.EasingStyle.Quad,Enum.EasingDirection.Out),
                     {Rotation = 0}
                 ):Play()
             else
                 isdropping = false
                 Dropdown:TweenSize(UDim2.new(0,470,0,31),"Out","Quad",0.3,true)
                 TweenService:Create(
                     DropImage,
                     TweenInfo.new(0.3,Enum.EasingStyle.Quad,Enum.EasingDirection.Out),
                     {Rotation = 180}
                 ):Play()
             end
         end)
    
         local dropfunc = {}
         function dropfunc:Add(t)
             local Item = Instance.new("TextButton")
             Item.Name = "Item"
             Item.Parent = DropScroll
             Item.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
             Item.BackgroundTransparency = 1.000
             Item.Size = UDim2.new(0, 470, 0, 26)
             Item.Font = Enum.Font.GothamSemibold
             Item.Text = tostring(t)
             Item.TextColor3 = Color3.fromRGB(225, 225, 225)
             Item.TextSize = 13.000
             Item.TextTransparency = 0.500
    
             Item.MouseEnter:Connect(function()
                 TweenService:Create(
                     Item,
                     TweenInfo.new(0.3,Enum.EasingStyle.Quad,Enum.EasingDirection.Out),
                     {TextTransparency = 0}
                 ):Play()
             end)
    
             Item.MouseLeave:Connect(function()
                 TweenService:Create(
                     Item,
                     TweenInfo.new(0.3,Enum.EasingStyle.Quad,Enum.EasingDirection.Out),
                     {TextTransparency = 0.5}
                 ):Play()
             end)
    
             Item.MouseButton1Click:Connect(function()
                 isdropping = false
                 Dropdown:TweenSize(UDim2.new(0,470,0,31),"Out","Quad",0.3,true)
                 TweenService:Create(
                     DropImage,
                     TweenInfo.new(0.3,Enum.EasingStyle.Quad,Enum.EasingDirection.Out),
                     {Rotation = 180}
                 ):Play()
                 callback(Item.Text)
                 DropTitle.Text = text.." : "..Item.Text
             end)
         end
         function dropfunc:Clear()
             DropTitle.Text = tostring(text).." : "
             isdropping = false
             Dropdown:TweenSize(UDim2.new(0,470,0,31),"Out","Quad",0.3,true)
             TweenService:Create(
                 DropImage,
                 TweenInfo.new(0.3,Enum.EasingStyle.Quad,Enum.EasingDirection.Out),
                 {Rotation = 180}
             ):Play()
             for i,v in next, DropScroll:GetChildren() do
                 if v:IsA("TextButton") then
                     v:Destroy()
                 end
             end
         end
         return dropfunc
     end
    
     function main:Slider(text,min,max,set,callback)
         local Slider = Instance.new("Frame")
         local slidercorner = Instance.new("UICorner")
         local sliderr = Instance.new("Frame")
         local sliderrcorner = Instance.new("UICorner")
         local SliderLabel = Instance.new("TextLabel")
         local HAHA = Instance.new("Frame")
         local AHEHE = Instance.new("TextButton")
         local bar = Instance.new("Frame")
         local bar1 = Instance.new("Frame")
         local bar1corner = Instance.new("UICorner")
         local barcorner = Instance.new("UICorner")
         local circlebar = Instance.new("Frame")
         local UICorner = Instance.new("UICorner")
         local slidervalue = Instance.new("Frame")
         local valuecorner = Instance.new("UICorner")
         local TextBox = Instance.new("TextBox")
         local UICorner_2 = Instance.new("UICorner")
    
         Slider.Name = "Slider"
         Slider.Parent = MainFramePage
         Slider.BackgroundColor3 = _G.Color
         Slider.BackgroundTransparency = 0
         Slider.Size = UDim2.new(0, 470, 0, 51)
    
         slidercorner.CornerRadius = UDim.new(0, 5)
         slidercorner.Name = "slidercorner"
         slidercorner.Parent = Slider
    
         sliderr.Name = "sliderr"
         sliderr.Parent = Slider
         sliderr.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
         sliderr.Position = UDim2.new(0, 1, 0, 1)
         sliderr.Size = UDim2.new(0, 468, 0, 49)
    
         sliderrcorner.CornerRadius = UDim.new(0, 5)
         sliderrcorner.Name = "sliderrcorner"
         sliderrcorner.Parent = sliderr
    
         SliderLabel.Name = "SliderLabel"
         SliderLabel.Parent = sliderr
         SliderLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
         SliderLabel.BackgroundTransparency = 1.000
         SliderLabel.Position = UDim2.new(0, 15, 0, 0)
         SliderLabel.Size = UDim2.new(0, 180, 0, 26)
         SliderLabel.Font = Enum.Font.GothamSemibold
         SliderLabel.Text = text
         SliderLabel.TextColor3 = Color3.fromRGB(225, 225, 225)
         SliderLabel.TextSize = 16.000
         SliderLabel.TextTransparency = 0
         SliderLabel.TextXAlignment = Enum.TextXAlignment.Left
    
         HAHA.Name = "HAHA"
         HAHA.Parent = sliderr
         HAHA.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
         HAHA.BackgroundTransparency = 1.000
         HAHA.Size = UDim2.new(0, 468, 0, 29)
    
         AHEHE.Name = "AHEHE"
         AHEHE.Parent = sliderr
         AHEHE.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
         AHEHE.BackgroundTransparency = 1.000
         AHEHE.Position = UDim2.new(0, 10, 0, 35)
         AHEHE.Size = UDim2.new(0, 448, 0, 5)
         AHEHE.Font = Enum.Font.SourceSans
         AHEHE.Text = ""
         AHEHE.TextColor3 = Color3.fromRGB(0, 0, 0)
         AHEHE.TextSize = 14.000
    
         bar.Name = "bar"
         bar.Parent = AHEHE
         bar.BackgroundColor3 = Color3.fromRGB(35, 35, 35)
         bar.Size = UDim2.new(0, 448, 0, 5)
    
         bar1.Name = "bar1"
         bar1.Parent = bar
         bar1.BackgroundColor3 = _G.Color
         bar1.BackgroundTransparency = 0
         bar1.Size = UDim2.new(set/max, 0, 0, 5)
    
         bar1corner.CornerRadius = UDim.new(0, 5)
         bar1corner.Name = "bar1corner"
         bar1corner.Parent = bar1
    
         barcorner.CornerRadius = UDim.new(0, 5)
         barcorner.Name = "barcorner"
         barcorner.Parent = bar
    
         circlebar.Name = "circlebar"
         circlebar.Parent = bar1
         circlebar.BackgroundColor3 = Color3.fromRGB(225, 225, 225)
         circlebar.Position = UDim2.new(1, -2, 0, -3)
         circlebar.Size = UDim2.new(0, 10, 0, 10)
    
         UICorner.CornerRadius = UDim.new(0, 100)
         UICorner.Parent = circlebar
    
         slidervalue.Name = "slidervalue"
         slidervalue.Parent = sliderr
         slidervalue.BackgroundColor3 = _G.Color
         slidervalue.BackgroundTransparency = 0
         slidervalue.Position = UDim2.new(0, 395, 0, 5)
         slidervalue.Size = UDim2.new(0, 65, 0, 18)
    
         valuecorner.CornerRadius = UDim.new(0, 5)
         valuecorner.Name = "valuecorner"
         valuecorner.Parent = slidervalue
    
         TextBox.Parent = slidervalue
         TextBox.BackgroundColor3 = Color3.fromRGB(35, 35, 35)
         TextBox.Position = UDim2.new(0, 1, 0, 1)
         TextBox.Size = UDim2.new(0, 63, 0, 16)
         TextBox.Font = Enum.Font.GothamSemibold
         TextBox.TextColor3 = Color3.fromRGB(225, 225, 225)
         TextBox.TextSize = 9.000
         TextBox.Text = set
         TextBox.TextTransparency = 0
    
         UICorner_2.CornerRadius = UDim.new(0, 5)
         UICorner_2.Parent = TextBox
    
         local mouse = game.Players.LocalPlayer:GetMouse()
         local uis = game:GetService("UserInputService")
    
         if Value == nil then
             Value = set
             pcall(function()
                 callback(Value)
             end)
         end
         
         AHEHE.MouseButton1Down:Connect(function()
             Value = math.floor((((tonumber(max) - tonumber(min)) / 448) * bar1.AbsoluteSize.X) + tonumber(min)) or 0
             pcall(function()
                 callback(Value)
             end)
             bar1.Size = UDim2.new(0, math.clamp(mouse.X - bar1.AbsolutePosition.X, 0, 448), 0, 5)
             circlebar.Position = UDim2.new(0, math.clamp(mouse.X - bar1.AbsolutePosition.X - 2, 0, 438), 0, -3)
             moveconnection = mouse.Move:Connect(function()
                 TextBox.Text = Value
                 Value = math.floor((((tonumber(max) - tonumber(min)) / 448) * bar1.AbsoluteSize.X) + tonumber(min))
                 pcall(function()
                     callback(Value)
                 end)
                 bar1.Size = UDim2.new(0, math.clamp(mouse.X - bar1.AbsolutePosition.X, 0, 448), 0, 5)
                 circlebar.Position = UDim2.new(0, math.clamp(mouse.X - bar1.AbsolutePosition.X - 2, 0, 438), 0, -3)
             end)
             releaseconnection = uis.InputEnded:Connect(function(Mouse)
                 if Mouse.UserInputType == Enum.UserInputType.MouseButton1 then
                     Value = math.floor((((tonumber(max) - tonumber(min)) / 448) * bar1.AbsoluteSize.X) + tonumber(min))
                     pcall(function()
                         callback(Value)
                     end)
                     bar1.Size = UDim2.new(0, math.clamp(mouse.X - bar1.AbsolutePosition.X, 0, 448), 0, 5)
                     circlebar.Position = UDim2.new(0, math.clamp(mouse.X - bar1.AbsolutePosition.X - 2, 0, 438), 0, -3)
                     moveconnection:Disconnect()
                     releaseconnection:Disconnect()
                 end
             end)
         end)
         releaseconnection = uis.InputEnded:Connect(function(Mouse)
             if Mouse.UserInputType == Enum.UserInputType.MouseButton1 then
                 Value = math.floor((((tonumber(max) - tonumber(min)) / 448) * bar1.AbsoluteSize.X) + tonumber(min))
                 TextBox.Text = Value
             end
         end)
    
         TextBox.FocusLost:Connect(function()
             if tonumber(TextBox.Text) > max then
                 TextBox.Text  = max
             end
             bar1.Size = UDim2.new((TextBox.Text or 0) / max, 0, 0, 5)
             circlebar.Position = UDim2.new(1, -2, 0, -3)
             TextBox.Text = tostring(TextBox.Text and math.floor( (TextBox.Text / max) * (max - min) + min) )
             pcall(callback, TextBox.Text)
         end)
     end
    
     function main:Textbox(text,disappear,callback)
         local Textbox = Instance.new("Frame")
         local TextboxCorner = Instance.new("UICorner")
         local Textboxx = Instance.new("Frame")
         local TextboxxCorner = Instance.new("UICorner")
         local TextboxLabel = Instance.new("TextLabel")
         local txtbtn = Instance.new("TextButton")
         local RealTextbox = Instance.new("TextBox")
         local UICorner = Instance.new("UICorner")
    
         Textbox.Name = "Textbox"
         Textbox.Parent = MainFramePage
         Textbox.BackgroundColor3 = _G.Color
         Textbox.BackgroundTransparency = 0
         Textbox.Size = UDim2.new(0, 470, 0, 31)
    
         TextboxCorner.CornerRadius = UDim.new(0, 5)
         TextboxCorner.Name = "TextboxCorner"
         TextboxCorner.Parent = Textbox
    
         Textboxx.Name = "Textboxx"
         Textboxx.Parent = Textbox
         Textboxx.BackgroundColor3 = Color3.fromRGB(45, 45, 45)
         Textboxx.Position = UDim2.new(0, 1, 0, 1)
         Textboxx.Size = UDim2.new(0, 468, 0, 29)
    
         TextboxxCorner.CornerRadius = UDim.new(0, 5)
         TextboxxCorner.Name = "TextboxxCorner"
         TextboxxCorner.Parent = Textboxx
    
         TextboxLabel.Name = "TextboxLabel"
         TextboxLabel.Parent = Textbox
         TextboxLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
         TextboxLabel.BackgroundTransparency = 1.000
         TextboxLabel.Position = UDim2.new(0, 15, 0, 0)
         TextboxLabel.Text = text
         TextboxLabel.Size = UDim2.new(0, 145, 0, 31)
         TextboxLabel.Font = Enum.Font.GothamSemibold
         TextboxLabel.TextColor3 = Color3.fromRGB(225, 225, 225)
         TextboxLabel.TextSize = 16.000
         TextboxLabel.TextTransparency = 0
         TextboxLabel.TextXAlignment = Enum.TextXAlignment.Left
    
         txtbtn.Name = "txtbtn"
         txtbtn.Parent = Textbox
         txtbtn.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
         txtbtn.BackgroundTransparency = 1.000
         txtbtn.Position = UDim2.new(0, 1, 0, 1)
         txtbtn.Size = UDim2.new(0, 468, 0, 29)
         txtbtn.Font = Enum.Font.SourceSans
         txtbtn.Text = ""
         txtbtn.TextColor3 = Color3.fromRGB(0, 0, 0)
         txtbtn.TextSize = 14.000
    
         RealTextbox.Name = "RealTextbox"
         RealTextbox.Parent = Textbox
         RealTextbox.BackgroundColor3 = Color3.fromRGB(35, 35, 35)
         RealTextbox.BackgroundTransparency = 0
         RealTextbox.Position = UDim2.new(0, 360, 0, 4)
         RealTextbox.Size = UDim2.new(0, 100, 0, 24)
         RealTextbox.Font = Enum.Font.GothamSemibold
         RealTextbox.Text = ""
         RealTextbox.TextColor3 = Color3.fromRGB(225, 225, 225)
         RealTextbox.TextSize = 11.000
         RealTextbox.TextTransparency = 0
    
         RealTextbox.FocusLost:Connect(function()
             callback(RealTextbox.Text)
             if disappear then
                 RealTextbox.Text = ""
             end
         end)
    
         UICorner.CornerRadius = UDim.new(0, 5)
         UICorner.Parent = RealTextbox
     end
     function main:Label(text)
         local Label = Instance.new("TextLabel")
         local PaddingLabel = Instance.new("UIPadding")
         local labelfunc = {}
    
         Label.Name = "Label"
         Label.Parent = MainFramePage
         Label.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
         Label.BackgroundTransparency = 1.000
         Label.Size = UDim2.new(0, 470, 0, 20)
         Label.Font = Enum.Font.GothamSemibold
         Label.TextColor3 = Color3.fromRGB(225, 225, 225)
         Label.TextSize = 16.000
         Label.Text = text
         Label.TextXAlignment = Enum.TextXAlignment.Left
    
         PaddingLabel.PaddingLeft = UDim.new(0,15)
         PaddingLabel.Parent = Label
         PaddingLabel.Name = "PaddingLabel"
    
         function labelfunc:Set(newtext)
             Label.Text = newtext
         end
         return labelfunc
     end
    
     function main:Seperator(text)
         local Seperator = Instance.new("Frame")
         local Sep1 = Instance.new("Frame")
         local Sep2 = Instance.new("TextLabel")
         local Sep3 = Instance.new("Frame")
         
         Seperator.Name = "Seperator"
         Seperator.Parent = MainFramePage
         Seperator.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
         Seperator.BackgroundTransparency = 1.000
         Seperator.Size = UDim2.new(0, 470, 0, 20)
         
         Sep1.Name = "Sep1"
         Sep1.Parent = Seperator
         Sep1.BackgroundColor3 = _G.Color
         Sep1.BorderSizePixel = 0
         Sep1.Position = UDim2.new(0, 0, 0, 10)
         Sep1.Size = UDim2.new(0, 80, 0, 1)
         
         Sep2.Name = "Sep2"
         Sep2.Parent = Seperator
         Sep2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
         Sep2.BackgroundTransparency = 1.000
         Sep2.Position = UDim2.new(0, 185, 0, 0)
         Sep2.Size = UDim2.new(0, 100, 0, 20)
         Sep2.Font = Enum.Font.GothamSemibold
         Sep2.Text = text
         Sep2.TextColor3 = Color3.fromRGB(255, 255, 255)
         Sep2.TextSize = 14.000
         
         Sep3.Name = "Sep3"
         Sep3.Parent = Seperator
         Sep3.BackgroundColor3 = _G.Color
         Sep3.BorderSizePixel = 0
         Sep3.Position = UDim2.new(0, 390, 0, 10)
         Sep3.Size = UDim2.new(0, 80, 0, 1)
     end
    
     function main:Line()
         local Linee = Instance.new("Frame")
         local Line = Instance.new("Frame")
         
         Linee.Name = "Linee"
         Linee.Parent = MainFramePage
         Linee.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
         Linee.BackgroundTransparency = 1.000
         Linee.Position = UDim2.new(0, 0, 0.119999997, 0)
         Linee.Size = UDim2.new(0, 470, 0, 20)
         
         Line.Name = "Line"
         Line.Parent = Linee
         Line.BackgroundColor3 = _G.Color
         Line.BorderSizePixel = 0
         Line.Position = UDim2.new(0, 0, 0, 10)
         Line.Size = UDim2.new(0, 470, 0, 1)
     end
     return main
    end
    return uitab
    end
    
    -- Function's
    -----------------------------------------------------------------------------------------
    
    spawn(function()
        while wait(.1) do
            if _G.AutoHaki then
                if game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
                else
                    local args = {
                        [1] = "Buso"
                    }
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                end
            end
            if _G.AutoHakiObs then
                if game.Players.LocalPlayer.PlayerGui.ScreenGui:FindFirstChild("ImageLabel") then
                else wait(1)
                    local virtualUser = game:GetService('VirtualUser')
                    virtualUser:CaptureController()
                    virtualUser:SetKeyDown('0x65')
                    wait(2)
                    virtualUser:SetKeyUp('0x65')
                end
            end
        end
    end)

    spawn(function()
        pcall(function()
        while wait() do
                if _G.AutoFarm or Auto_Bone or _G.AutoAllBoss or _G.AutoFarmBoss or _G.AutoAllBossHop or _G.TeleportPly or _G.AutoRaid or _G.AutoFarmGunMastery or _G.AutoFarmFruitMastery == true then
                    if not game:GetService("Players").LocalPlayer.Character.HumanoidRootPart:FindFirstChild("BodyClip") then
                        local Noclip = Instance.new("BodyVelocity")
                        Noclip.Name = "BodyClip"
                        Noclip.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
                        Noclip.MaxForce = Vector3.new(100000,100000,100000)
                        Noclip.Velocity = Vector3.new(0,0,0)
                    end
                end
            end
        end)
    end)
    spawn(function()
        pcall(function()
            while wait() do
                if _G.AutoFarm == true then
                for _, v in pairs(game:GetService("Players").LocalPlayer.Character:GetDescendants()) do
                        if v:IsA("BasePart") then
                        v.CanCollide = false    
                    end
                end
            end
        end
    end)
    end)

    spawn(function()
        pcall(function()
            while wait() do
                if _G.WalkOnWater or _G.AutoFarm then
                    if game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame.Y <= 1 then
                        if not game:GetService("Workspace"):FindFirstChild("Water") then
                            local Water = Instance.new("Part", game:GetService("Workspace"))
                            Water.Name = "Water"
                            Water.Size = Vector3.new(15,0.5,15)
                            Water.Anchored = true
                            Water.Material = "Neon"
                            Water.Color = _G.Color
                            game:GetService("Workspace").Water.CFrame = CFrame.new(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame.X,game:GetService("Workspace").Camera["Water;"].CFrame.Y,game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame.Z)
                        else
                            game:GetService("Workspace").Water.CFrame = CFrame.new(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame.X,game:GetService("Workspace").Camera["Water;"].CFrame.Y,game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame.Z)
                        end
                    elseif game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame.Y >= 1 and game:GetService("Workspace"):FindFirstChild("Water") then
                        game:GetService("Workspace"):FindFirstChild("Water"):Destroy()
                    end
                else
                    if game:GetService("Workspace"):FindFirstChild("Water") then
                        game:GetService("Workspace"):FindFirstChild("Water"):Destroy()
                    end
                end
            end
        end)
    end)
    
    spawn(function()
        game:GetService("RunService").Heartbeat:Connect(function()
            if _G.AutoFarm then
                if not game:GetService("Workspace"):FindFirstChild("PartNino") then
                    local LOL = Instance.new("Part")
                    LOL.Name = "PartNino"
                    LOL.Parent = game.Workspace
                    LOL.Anchored = true
                    LOL.Transparency = 1
                    LOL.Size = Vector3.new(30,1,30)
            elseif game:GetService("Workspace"):FindFirstChild("PartNino") then
                    game.Workspace["PartNino"].CFrame = CFrame.new(game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame.X,game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame.Y - 3.92,game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame.Z)
                end
            else
                if game:GetService("Workspace"):FindFirstChild("PartNino") then
                    game:GetService("Workspace"):FindFirstChild("PartNino"):Destroy()
                end
            end
        end)
    end)
    
    game:GetService("RunService").Heartbeat:Connect(function()
        for i,v in pairs(game:GetService("Workspace")["_WorldOrigin"]:GetChildren()) do
            pcall(function()
                if v.Name == ("CurvedRing") or v.Name == ("SlashHit") or v.Name == ("DamageCounter") or v.Name == ("SwordSlash") or v.Name == ("SlashTail") or v.Name == ("Sounds") then
                    v:Destroy()
                end
            end)
        end
    end)
    
    local CameraShaker = require(game.ReplicatedStorage.Util.CameraShaker)
    CombatFrameworkZ = require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework)
    y = debug.getupvalues(CombatFrameworkZ)[2]
    local yAttack = 0.1
    spawn(function()
        game:GetService("RunService").RenderStepped:Connect(function()
            if _G.FastAttack then
                if typeof(y) == "table" then
                    pcall(function()
                        CameraShaker:Stop()
                        y.activeController.timeToNextAttack = (math.huge^math.huge^math.huge)
                        y.activeController.timeToNextAttack = 0.1
                        y.activeController.hitboxMagnitude = 120
                        y.activeController.timeToNextBlock = 0
                        y.activeController.focusStart = 0
                        y.activeController.increment = 3
                        y.activeController.blocking = false
                        y.activeController.attacking = false
                        y.activeController.humanoid.AutoRotate = true
                    end)
                end
            end
        end)
    end)

    spawn(function()
        while task.wait() do
            pcall(function()
                if Magnet then
                    CheckQuest()
                    for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                        if _G.AutoFarm and MagnetActive and v.Name == Mon and (Mon == "Factory Staff [Lv. 800]" or Mon == "Monkey [Lv. 14]" or Mon == "Dragon Crew Warrior [Lv. 1575]" or Mon == "Dragon Crew Archer [Lv. 1600]") and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and (v.HumanoidRootPart.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 220 then
                            v.HumanoidRootPart.Size = Vector3.new(80,80,80)
                            v.HumanoidRootPart.CFrame = PosMon
                            v.Humanoid:ChangeState(14)
                            v.HumanoidRootPart.CanCollide = false
                            v.Head.CanCollide = false
                            if v.Humanoid:FindFirstChild("Animator") then
                            v.Humanoid.Animator:Destroy()
                            end
                            sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
                        elseif _G.AutoFarm and MagnetActive and v.Name == Mon and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 and (v.HumanoidRootPart.Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 275 then
                            v.HumanoidRootPart.Size = Vector3.new(80,80,80)
                            v.HumanoidRootPart.CFrame = PosMon
                            v.Humanoid:ChangeState(14)
                            v.HumanoidRootPart.CanCollide = false
                            v.Head.CanCollide = false
                            if v.Humanoid:FindFirstChild("Animator") then
                            v.Humanoid.Animator:Destroy()
                            end
                            sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
                        elseif _G.AutoBone and BoneMagnet and Magnet then
                            if (v.Name == "Reborn Skeleton [Lv. 1975]" or v.Name == "Living Zombie [Lv. 2000]" or v.Name == "Demonic Soul [Lv. 2025]" or v.Name == "Posessed Mummy [Lv. 2050]") and (v.HumanoidRootPart.Position - MainMonBone.Position).Magnitude <= 300 then
                            v.Head.CanCollide = false
                            v.HumanoidRootPart.CanCollide = false
                            v.Humanoid:ChangeState(14)
                            v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
                            v.HumanoidRootPart.CFrame = MainMonBone
                            elseif v.Humanoid:FindFirstChild("Animator") then
                            v.Humanoid.Animator:Destroy()
                            if sethiddenproperty then 
                            sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius",  10000)
                            end
                            sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
                            end
                        end
                    end
                end
            end)
        end
    end)

    -- Main Script's
    local Library = Update:Window("    SHADOW","",Enum.KeyCode.RightControl);
    Main = Library:Tab("Main")
    Stats = Library:Tab("Stats")
    Shop = Library:Tab("Shop")
    Island = Library:Tab("Island")
    Player = Library:Tab("Player")
    Dungeon = Library:Tab("Dungeon")
    Misc = Library:Tab("Miscellaneous")
    Main:Seperator("Main")
    -------------------------------------------------------------------------------------------
    function CheckLevel()
        local Lv = game:GetService("Players").LocalPlayer.Data.Level.Value
        if Old_World then
            if Lv == 1 or Lv <= 9 or SelectMonster == "Bandit [Lv. 5]" then -- Bandit
                Ms = "Bandit [Lv. 5]"
                NameQuest = "BanditQuest1"
                QuestLv = 1
                NameMon = "Bandit"
                CFrameQ = CFrame.new(1060.9383544922, 16.455066680908, 1547.7841796875)
                CFrameMon = CFrame.new(1038.5533447266, 41.296249389648, 1576.5098876953)
            elseif Lv == 10 or Lv <= 14 or SelectMonster == "Monkey [Lv. 14]" then -- Monkey
                Ms = "Monkey [Lv. 14]"
                NameQuest = "JungleQuest"
                QuestLv = 1
                NameMon = "Monkey"
                CFrameQ = CFrame.new(-1601.6553955078, 36.85213470459, 153.38809204102)
                CFrameMon = CFrame.new(-1448.1446533203, 50.851993560791, 63.60718536377)
            elseif Lv == 15 or Lv <= 29 or SelectMonster == "Gorilla [Lv. 20]" then -- Gorilla
                Ms = "Gorilla [Lv. 20]"
                NameQuest = "JungleQuest"
                QuestLv = 2
                NameMon = "Gorilla"
                CFrameQ = CFrame.new(-1601.6553955078, 36.85213470459, 153.38809204102)
                CFrameMon = CFrame.new(-1142.6488037109, 40.462348937988, -515.39227294922)
            elseif Lv == 30 or Lv <= 39 or SelectMonster == "Pirate [Lv. 35]" then -- Pirate
                Ms = "Pirate [Lv. 35]"
                NameQuest = "BuggyQuest1"
                QuestLv = 1
                NameMon = "Pirate"
                CFrameQ = CFrame.new(-1140.1761474609, 4.752049446106, 3827.4057617188)
                CFrameMon = CFrame.new(-1201.0881347656, 40.628940582275, 3857.5966796875)
            elseif Lv == 40 or Lv <= 59 or SelectMonster == "Brute [Lv. 45]" then -- Brute
                Ms = "Brute [Lv. 45]"
                NameQuest = "BuggyQuest1"
                QuestLv = 2
                NameMon = "Brute"
                CFrameQ = CFrame.new(-1140.1761474609, 4.752049446106, 3827.4057617188)
                CFrameMon = CFrame.new(-1387.5324707031, 24.592035293579, 4100.9575195313)
            elseif Lv == 60 or Lv <= 74 or SelectMonster == "Desert Bandit [Lv. 60]" then -- Desert Bandit
                Ms = "Desert Bandit [Lv. 60]"
                NameQuest = "DesertQuest"
                QuestLv = 1
                NameMon = "Desert Bandit"
                CFrameQ = CFrame.new(896.51721191406, 6.4384617805481, 4390.1494140625)
                CFrameMon = CFrame.new(984.99896240234, 16.109552383423, 4417.91015625)
            elseif Lv == 75 or Lv <= 89 or SelectMonster == "Desert Officer [Lv. 70]" then -- Desert Officer
                Ms = "Desert Officer [Lv. 70]"
                NameQuest = "DesertQuest"
                QuestLv = 2
                NameMon = "Desert Officer"
                CFrameQ = CFrame.new(896.51721191406, 6.4384617805481, 4390.1494140625)
                CFrameMon = CFrame.new(1547.1510009766, 14.452038764954, 4381.8002929688)
            elseif Lv == 90 or Lv <= 99 or SelectMonster == "Snow Bandit [Lv. 90]" then -- Snow Bandit
                Ms = "Snow Bandit [Lv. 90]"
                NameQuest = "SnowQuest"
                QuestLv = 1
                NameMon = "Snow Bandit"
                CFrameQ = CFrame.new(1386.8073730469, 87.272789001465, -1298.3576660156)
                CFrameMon = CFrame.new(1356.3028564453, 105.76865386963, -1328.2418212891)
            elseif Lv == 100 or Lv <= 119 or SelectMonster == "Snowman [Lv. 100]" then -- Snowman
                Ms = "Snowman [Lv. 100]"
                NameQuest = "SnowQuest"
                QuestLv = 2
                NameMon = "Snowman"
                CFrameQ = CFrame.new(1386.8073730469, 87.272789001465, -1298.3576660156)
                CFrameMon = CFrame.new(1218.7956542969, 138.01184082031, -1488.0262451172)
            elseif Lv == 120 or Lv <= 149 or SelectMonster == "Chief Petty Officer [Lv. 120]" then -- Chief Petty Officer
                Ms = "Chief Petty Officer [Lv. 120]"
                NameQuest = "MarineQuest2"
                QuestLv = 1
                NameMon = "Chief Petty Officer"
                CFrameQ = CFrame.new(-5035.49609375, 28.677835464478, 4324.1840820313)
                CFrameMon = CFrame.new(-4931.1552734375, 65.793113708496, 4121.8393554688)
            elseif Lv == 150 or Lv <= 174 or SelectMonster == "Sky Bandit [Lv. 150]" then -- Sky Bandit
                Ms = "Sky Bandit [Lv. 150]"
                NameQuest = "SkyQuest"
                QuestLv = 1
                NameMon = "Sky Bandit"
                CFrameQ = CFrame.new(-4842.1372070313, 717.69543457031, -2623.0483398438)
                CFrameMon = CFrame.new(-4955.6411132813, 365.46365356445, -2908.1865234375)
            elseif Lv == 175 or Lv <= 179 or SelectMonster == "Dark Master [Lv. 175]" then -- Dark Master
                Ms = "Dark Master [Lv. 175]"
                NameQuest = "SkyQuest"
                QuestLv = 2
                NameMon = "Dark Master"
                CFrameQ = CFrame.new(-4842.1372070313, 717.69543457031, -2623.0483398438)
                CFrameMon = CFrame.new(-5148.1650390625, 439.04571533203, -2332.9611816406)
               elseif Lv == 180 or Lv <= 209 or SelectMonster == "Prisoner [Lv. 190]" then -- Prisoner
               Ms = "Prisoner [Lv. 190]"
               NameQuest = "PrisonerQuest"
               QuestLv = 1
               NameMon = "Prisoner"
               CFrameQ = CFrame.new(5309.3584, 2.1345036, 474.173645, -0.273264647, -9.34814608e-08, -0.961938918, 3.1041214e-09, 1, -9.80620527e-08, 0.961938918, -2.97828677e-08, -0.273264647)
               CFrameMon = CFrame.new(5393.40723, 15.6333637, 486.675385, -0.748236716, 2.00700012e-09, -0.663431823, -8.54028226e-09, 1, 1.26571456e-08, 0.663431823, 1.51364361e-08, -0.748236716)
               elseif Lv == 210 or Lv <= 249 or SelectMonster == "Dangerous Prisoner [Lv. 210]" then -- Dangerous
               Ms = "Dangerous Prisoner [Lv. 210]"
               NameQuest = "PrisonerQuest"
               QuestLv = 2
               NameMon = "Dangerous Prisoner"
               CFrameQ = CFrame.new(5309.3584, 2.1345036, 474.173645, -0.273264647, -9.34814608e-08, -0.961938918, 3.1041214e-09, 1, -9.80620527e-08, 0.961938918, -2.97828677e-08, -0.273264647)
               CFrameMon = CFrame.new(5393.40723, 15.6333637, 486.675385, -0.748236716, 2.00700012e-09, -0.663431823, -8.54028226e-09, 1, 1.26571456e-08, 0.663431823, 1.51364361e-08, -0.748236716)
            elseif Lv == 250 or Lv <= 274 or SelectMonster == "Toga Warrior [Lv. 250]" then -- Toga Warrior
                Ms = "Toga Warrior [Lv. 250]"
                NameQuest = "ColosseumQuest"
                QuestLv = 1
                NameMon = "Toga Warrior"
                CFrameQ = CFrame.new(-1577.7890625, 7.4151420593262, -2984.4838867188)
                CFrameMon = CFrame.new(-1872.5166015625, 49.080215454102, -2913.810546875)
            elseif Lv == 275 or Lv <= 299 or SelectMonster == "Gladiator [Lv. 275]" then -- Gladiator
                Ms = "Gladiator [Lv. 275]"
                NameQuest = "ColosseumQuest"
                QuestLv = 2
                NameMon = "Gladiator"
                CFrameQ = CFrame.new(-1577.7890625, 7.4151420593262, -2984.4838867188)
                CFrameMon = CFrame.new(-1521.3740234375, 81.203170776367, -3066.3139648438)
            elseif Lv == 300 or Lv <= 324 or SelectMonster == "Military Soldier [Lv. 300]" then -- Military Soldier
                Ms = "Military Soldier [Lv. 300]"
                NameQuest = "MagmaQuest"
                QuestLv = 1
                NameMon = "Military Soldier"
                CFrameQ = CFrame.new(-5316.1157226563, 12.262831687927, 8517.00390625)
                CFrameMon = CFrame.new(-5369.0004882813, 61.24352645874, 8556.4921875)
            elseif Lv == 325 or Lv <= 374 or SelectMonster == "Military Spy [Lv. 325]" then -- Military Spy
                Ms = "Military Spy [Lv. 325]"
                NameQuest = "MagmaQuest"
                QuestLv = 2
                NameMon = "Military Spy"
                CFrameQ = CFrame.new(-5316.1157226563, 12.262831687927, 8517.00390625)
                CFrameMon = CFrame.new(-5984.0532226563, 82.14656829834, 8753.326171875)
            elseif Lv == 375 or Lv <= 399 or SelectMonster == "Fishman Warrior [Lv. 375]" then -- Fishman Warrior 
                Ms = "Fishman Warrior [Lv. 375]"
                NameQuest = "FishmanQuest"
                QuestLv = 1
                NameMon = "Fishman Warrior"
                CFrameQ = CFrame.new(61122.65234375, 18.497442245483, 1569.3997802734)
                CFrameMon = CFrame.new(60844.10546875, 98.462875366211, 1298.3985595703)
                if Auto_Farm and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 3000 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(61163.8515625, 11.6796875, 1819.7841796875))
                end
            elseif Lv == 400 or Lv <= 449 or SelectMonster == "Fishman Commando [Lv. 400]" then -- Fishman Commando
                Ms = "Fishman Commando [Lv. 400]"
                NameQuest = "FishmanQuest"
                QuestLv = 2
                NameMon = "Fishman Commando"
                CFrameQ = CFrame.new(61122.65234375, 18.497442245483, 1569.3997802734)
                CFrameMon = CFrame.new(61738.3984375, 64.207321166992, 1433.8375244141)
                if Auto_Farm and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 3000 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(61163.8515625, 11.6796875, 1819.7841796875))
                end
            elseif Lv == 450 or Lv <= 474 or SelectMonster == "God's Guard [Lv. 450]" then -- God's Guard
                Ms = "God's Guard [Lv. 450]"
                NameQuest = "SkyExp1Quest"
                QuestLv = 1
                NameMon = "God's Guard"
                CFrameQ = CFrame.new(-4721.8603515625, 845.30297851563, -1953.8489990234)
                CFrameMon = CFrame.new(-4628.0498046875, 866.92877197266, -1931.2352294922)
                if Auto_Farm and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 3000 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(-4607.82275, 872.54248, -1667.55688))
                end
            elseif Lv == 475 or Lv <= 524 or SelectMonster == "Shanda [Lv. 475]" then -- Shanda
                Ms = "Shanda [Lv. 475]"
                NameQuest = "SkyExp1Quest"
                QuestLv = 2
                NameMon = "Shanda"
                CFrameQ = CFrame.new(-7863.1596679688, 5545.5190429688, -378.42266845703)
                CFrameMon = CFrame.new(-7685.1474609375, 5601.0751953125, -441.38876342773)
                if Auto_Farm and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 3000 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(-7894.6176757813, 5547.1416015625, -380.29119873047))
                end
            elseif Lv == 525 or Lv <= 549 or SelectMonster == "Royal Squad [Lv. 525]" then -- Royal Squad
                Ms = "Royal Squad [Lv. 525]"
                NameQuest = "SkyExp2Quest"
                QuestLv = 1
                NameMon = "Royal Squad"
                CFrameQ = CFrame.new(-7903.3828125, 5635.9897460938, -1410.923828125)
                CFrameMon = CFrame.new(-7654.2514648438, 5637.1079101563, -1407.7550048828)
            elseif Lv == 550 or Lv <= 624 or SelectMonster == "Royal Soldier [Lv. 550]" then -- Royal Soldier
                Ms = "Royal Soldier [Lv. 550]"
                NameQuest = "SkyExp2Quest"
                QuestLv = 2
                NameMon = "Royal Soldier"
                CFrameQ = CFrame.new(-7903.3828125, 5635.9897460938, -1410.923828125)
                CFrameMon = CFrame.new(-7760.4106445313, 5679.9077148438, -1884.8112792969)
            elseif Lv == 625 or Lv <= 649 or SelectMonster == "Galley Pirate [Lv. 625]" then -- Galley Pirate
                Ms = "Galley Pirate [Lv. 625]"
                NameQuest = "FountainQuest"
                QuestLv = 1
                NameMon = "Galley Pirate"
                CFrameQ = CFrame.new(5258.2788085938, 38.526931762695, 4050.044921875)
                CFrameMon = CFrame.new(5557.1684570313, 152.32717895508, 3998.7758789063)
            elseif Lv >= 650 or SelectMonster == "Galley Captain [Lv. 650]" then -- Galley Captain
                Ms = "Galley Captain [Lv. 650]"
                NameQuest = "FountainQuest"
                QuestLv = 2
                NameMon = "Galley Captain"
                CFrameQ = CFrame.new(5258.2788085938, 38.526931762695, 4050.044921875)
                CFrameMon = CFrame.new(5677.6772460938, 92.786109924316, 4966.6323242188)
            end
        end
        if New_World then
            if Lv == 700 or Lv <= 724 or SelectMonster == "Raider [Lv. 700]" then -- Raider
                Ms = "Raider [Lv. 700]"
                NameQuest = "Area1Quest"
                QuestLv = 1
                NameMon = "Raider"
                CFrameQ = CFrame.new(-427.72567749023, 72.99634552002, 1835.9426269531)
                CFrameMon = CFrame.new(68.874565124512, 93.635643005371, 2429.6752929688)
            elseif Lv == 725 or Lv <= 774 or SelectMonster == "Mercenary [Lv. 725]" then -- Mercenary
                Ms = "Mercenary [Lv. 725]"
                NameQuest = "Area1Quest"
                QuestLv = 2
                NameMon = "Mercenary"
                CFrameQ = CFrame.new(-427.72567749023, 72.99634552002, 1835.9426269531)
                CFrameMon = CFrame.new(-864.85009765625, 122.47104644775, 1453.1505126953)
            elseif Lv == 775 or Lv <= 799 or SelectMonster == "Swan Pirate [Lv. 775]" then -- Swan Pirate
                Ms = "Swan Pirate [Lv. 775]"
                NameQuest = "Area2Quest"
                QuestLv = 1
                NameMon = "Swan Pirate"
                CFrameQ = CFrame.new(635.61151123047, 73.096351623535, 917.81298828125)
                CFrameMon = CFrame.new(1065.3669433594, 137.64012145996, 1324.3798828125)
            elseif Lv == 800 or Lv <= 874 or SelectMonster == "Factory Staff [Lv. 800]" then -- Factory Staff
                Ms = "Factory Staff [Lv. 800]"
                NameQuest = "Area2Quest"
                QuestLv = 2
                NameMon = "Factory Staff"
                CFrameQ = CFrame.new(635.61151123047, 73.096351623535, 917.81298828125)
                CFrameMon = CFrame.new(533.22045898438, 128.46876525879, 355.62615966797)
            elseif Lv == 875 or Lv <= 899 or SelectMonster == "Marine Lieutenant [Lv. 875]" then -- Marine Lieutenant
                Ms = "Marine Lieutenant [Lv. 875]"
                NameQuest = "MarineQuest3"
                QuestLv = 1
                NameMon = "Marine Lieutenant"
                CFrameQ = CFrame.new(-2440.9934082031, 73.04190826416, -3217.7082519531)
                CFrameMon = CFrame.new(-2489.2622070313, 84.613594055176, -3151.8830566406)
            elseif Lv == 900 or Lv <= 949 or SelectMonster == "Marine Captain [Lv. 900]" then -- Marine Captain
                Ms = "Marine Captain [Lv. 900]"
                NameQuest = "MarineQuest3"
                QuestLv = 2
                NameMon = "Marine Captain"
                CFrameQ = CFrame.new(-2440.9934082031, 73.04190826416, -3217.7082519531)
                CFrameMon = CFrame.new(-2335.2026367188, 79.786659240723, -3245.8674316406)
            elseif Lv == 950 or Lv <= 974 or SelectMonster == "Zombie [Lv. 950]" then -- Zombie
                Ms = "Zombie [Lv. 950]"
                NameQuest = "ZombieQuest"
                QuestLv = 1
                NameMon = "Zombie"
                CFrameQ = CFrame.new(-5494.3413085938, 48.505931854248, -794.59094238281)
                CFrameMon = CFrame.new(-5536.4970703125, 101.08577728271, -835.59075927734)
            elseif Lv == 975 or Lv <= 999 or SelectMonster == "Vampire [Lv. 975]" then -- Vampire
                Ms = "Vampire [Lv. 975]"
                NameQuest = "ZombieQuest"
                QuestLv = 2
                NameMon = "Vampire"
                CFrameQ = CFrame.new(-5494.3413085938, 48.505931854248, -794.59094238281)
                CFrameMon = CFrame.new(-5806.1098632813, 16.722528457642, -1164.4384765625)
            elseif Lv == 1000 or Lv <= 1049 or SelectMonster == "Snow Trooper [Lv. 1000]" then -- Snow Trooper
                Ms = "Snow Trooper [Lv. 1000]"
                NameQuest = "SnowMountainQuest"
                QuestLv = 1
                NameMon = "Snow Trooper"
                CFrameQ = CFrame.new(607.05963134766, 401.44781494141, -5370.5546875)
                CFrameMon = CFrame.new(535.21051025391, 432.74209594727, -5484.9165039063)
            elseif Lv == 1050 or Lv <= 1099 or SelectMonster == "Winter Warrior [Lv. 1050]" then -- Winter Warrior
                Ms = "Winter Warrior [Lv. 1050]"
                NameQuest = "SnowMountainQuest"
                QuestLv = 2
                NameMon = "Winter Warrior"
                CFrameQ = CFrame.new(607.05963134766, 401.44781494141, -5370.5546875)
                CFrameMon = CFrame.new(1234.4449462891, 456.95419311523, -5174.130859375)
            elseif Lv == 1100 or Lv <= 1124 or SelectMonster == "Lab Subordinate [Lv. 1100]" then -- Lab Subordinate
                Ms = "Lab Subordinate [Lv. 1100]"
                NameQuest = "IceSideQuest"
                QuestLv = 1
                NameMon = "Lab Subordinate"
                CFrameQ = CFrame.new(-6061.841796875, 15.926671981812, -4902.0385742188)
                CFrameMon = CFrame.new(-5720.5576171875, 63.309471130371, -4784.6103515625)
            elseif Lv == 1125 or Lv <= 1174 or SelectMonster == "Horned Warrior [Lv. 1125]" then -- Horned Warrior
                Ms = "Horned Warrior [Lv. 1125]"
                NameQuest = "IceSideQuest"
                QuestLv = 2
                NameMon = "Horned Warrior"
                CFrameQ = CFrame.new(-6061.841796875, 15.926671981812, -4902.0385742188)
                CFrameMon = CFrame.new(-6292.751953125, 91.181983947754, -5502.6499023438)
            elseif Lv == 1175 or Lv <= 1199 or SelectMonster == "Magma Ninja [Lv. 1175]" then -- Magma Ninja
                Ms = "Magma Ninja [Lv. 1175]"
                NameQuest = "FireSideQuest"
                QuestLv = 1
                NameMon = "Magma Ninja"
                CFrameQ = CFrame.new(-5429.0473632813, 15.977565765381, -5297.9614257813)
                CFrameMon = CFrame.new(-5461.8388671875, 130.36347961426, -5836.4702148438)
            elseif Lv == 1200 or Lv <= 1249 or SelectMonster == "Lava Pirate [Lv. 1200]" then -- Lava Pirate
                Ms = "Lava Pirate [Lv. 1200]"
                NameQuest = "FireSideQuest"
                QuestLv = 2
                NameMon = "Lava Pirate"
                CFrameQ = CFrame.new(-5429.0473632813, 15.977565765381, -5297.9614257813)
                CFrameMon = CFrame.new(-5251.1889648438, 55.164535522461, -4774.4096679688)
            elseif Lv == 1250 or Lv <= 1274 or SelectMonster == "Ship Deckhand [Lv. 1250]" then -- Ship Deckhand
                Ms = "Ship Deckhand [Lv. 1250]"
                NameQuest = "ShipQuest1"
                QuestLv = 1
                NameMon = "Ship Deckhand"
                CFrameQ = CFrame.new(1040.2927246094, 125.08293151855, 32911.0390625)
                CFrameMon = CFrame.new(921.12365722656, 125.9839553833, 33088.328125)
                if Auto_Farm and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 20000 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(923.21252441406, 126.9760055542, 32852.83203125))
                end
            elseif Lv == 1275 or Lv <= 1299 or SelectMonster == "Ship Engineer [Lv. 1275]" then -- Ship Engineer
                Ms = "Ship Engineer [Lv. 1275]"
                NameQuest = "ShipQuest1"
                QuestLv = 2
                NameMon = "Ship Engineer"
                CFrameQ = CFrame.new(1040.2927246094, 125.08293151855, 32911.0390625)
                CFrameMon = CFrame.new(886.28179931641, 40.47790145874, 32800.83203125)
                if Auto_Farm and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 20000 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(923.21252441406, 126.9760055542, 32852.83203125))
                end
            elseif Lv == 1300 or Lv <= 1324 or SelectMonster == "Ship Steward [Lv. 1300]" then -- Ship Steward
                Ms = "Ship Steward [Lv. 1300]"
                NameQuest = "ShipQuest2"
                QuestLv = 1
                NameMon = "Ship Steward"
                CFrameQ = CFrame.new(971.42065429688, 125.08293151855, 33245.54296875)
                CFrameMon = CFrame.new(943.85504150391, 129.58183288574, 33444.3671875)
                if Auto_Farm and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 20000 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(923.21252441406, 126.9760055542, 32852.83203125))
                end
            elseif Lv == 1325 or Lv <= 1349 or SelectMonster == "Ship Officer [Lv. 1325]" then -- Ship Officer
                Ms = "Ship Officer [Lv. 1325]"
                NameQuest = "ShipQuest2"
                QuestLv = 2
                NameMon = "Ship Officer"
                CFrameQ = CFrame.new(971.42065429688, 125.08293151855, 33245.54296875)
                CFrameMon = CFrame.new(955.38458251953, 181.08335876465, 33331.890625)
                if Auto_Farm and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 20000 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(923.21252441406, 126.9760055542, 32852.83203125))
                end
            elseif Lv == 1350 or Lv <= 1374 or SelectMonster == "Arctic Warrior [Lv. 1350]" then -- Arctic Warrior
                Ms = "Arctic Warrior [Lv. 1350]"
                NameQuest = "FrostQuest"
                QuestLv = 1
                NameMon = "Arctic Warrior"
                CFrameQ = CFrame.new(5668.1372070313, 28.202531814575, -6484.6005859375)
                CFrameMon = CFrame.new(5935.4541015625, 77.26016998291, -6472.7568359375)
                if Auto_Farm and (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 20000 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(-6508.5581054688, 89.034996032715, -132.83953857422))
                end
            elseif Lv == 1375 or Lv <= 1424 or SelectMonster == "Snow Lurker [Lv. 1375]" then -- Snow Lurker
                Ms = "Snow Lurker [Lv. 1375]"
                NameQuest = "FrostQuest"
                QuestLv = 2
                NameMon = "Snow Lurker"
                CFrameQ = CFrame.new(5668.1372070313, 28.202531814575, -6484.6005859375)
                CFrameMon = CFrame.new(5628.482421875, 57.574996948242, -6618.3481445313)
            elseif Lv == 1425 or Lv <= 1449 or SelectMonster == "Sea Soldier [Lv. 1425]" then -- Sea Soldier
                Ms = "Sea Soldier [Lv. 1425]"
                NameQuest = "ForgottenQuest"
                QuestLv = 1
                NameMon = "Sea Soldier"
                CFrameQ = CFrame.new(-3054.5827636719, 236.87213134766, -10147.790039063)
                CFrameMon = CFrame.new(-3185.0153808594, 58.789089202881, -9663.6064453125)
            elseif Lv >= 1450 or SelectMonster == "Water Fighter [Lv. 1450]" then -- Water Fighter
                Ms = "Water Fighter [Lv. 1450]"
                NameQuest = "ForgottenQuest"
                QuestLv = 2
                NameMon = "Water Fighter"
                CFrameQ = CFrame.new(-3054.5827636719, 236.87213134766, -10147.790039063)
                CFrameMon = CFrame.new(-3262.9301757813, 298.69036865234, -10552.529296875)
            end
        end
        if Three_World then
            if Lv == 1500 or Lv <= 1524 or SelectMonster == "Pirate Millionaire [Lv. 1500]" then -- Pirate Millionaire
                Ms = "Pirate Millionaire [Lv. 1500]"
                NameQuest = "PiratePortQuest"
                QuestLv = 1
                NameMon = "Pirate Millionaire"
                CFrameQ = CFrame.new(-289.61752319336, 43.819011688232, 5580.0903320313)
                CFrameMon = CFrame.new(-435.68109130859, 189.69866943359, 5551.0756835938)
            elseif Lv == 1525 or Lv <= 1574 or SelectMonster == "Pistol Billionaire [Lv. 1525]" then -- Pistol Billoonaire
                Ms = "Pistol Billionaire [Lv. 1525]"
                NameQuest = "PiratePortQuest"
                QuestLv = 2
                NameMon = "Pistol Billionaire"
                CFrameQ = CFrame.new(-289.61752319336, 43.819011688232, 5580.0903320313)
                CFrameMon = CFrame.new(-236.53652954102, 217.46676635742, 6006.0883789063)
            elseif Lv == 1575 or Lv <= 1599 or SelectMonster == "Dragon Crew Warrior [Lv. 1575]" then -- Dragon Crew Warrior
                Ms = "Dragon Crew Warrior [Lv. 1575]"
                NameQuest = "AmazonQuest"
                QuestLv = 1
                NameMon = "Dragon Crew Warrior"
                CFrameQ = CFrame.new(5833.1147460938, 51.60498046875, -1103.0693359375)
                CFrameMon = CFrame.new(6301.9975585938, 104.77153015137, -1082.6075439453)
            elseif Lv == 1600 or Lv <= 1624 or SelectMonster == "Dragon Crew Archer [Lv. 1600]" then -- Dragon Crew Archer
                Ms = "Dragon Crew Archer [Lv. 1600]"
                NameQuest = "AmazonQuest"
                QuestLv = 2
                NameMon = "Dragon Crew Archer"
                CFrameQ = CFrame.new(5833.1147460938, 51.60498046875, -1103.0693359375)
                CFrameMon = CFrame.new(6831.1171875, 441.76708984375, 446.58615112305)
            elseif Lv == 1625 or Lv <= 1649 or SelectMonster == "Female Islander [Lv. 1625]" then -- Female Islander
                Ms = "Female Islander [Lv. 1625]"
                NameQuest = "AmazonQuest2"
                QuestLv = 1
                NameMon = "Female Islander"
                CFrameQ = CFrame.new(5446.8793945313, 601.62945556641, 749.45672607422)
                CFrameMon = CFrame.new(5792.5166015625, 848.14392089844, 1084.1818847656)
            elseif Lv == 1650 or Lv <= 1699 or SelectMonster == "Giant Islander [Lv. 1650]" then -- Giant Islander
                Ms = "Giant Islander [Lv. 1650]"
                NameQuest = "AmazonQuest2"
                QuestLv = 2
                NameMon = "Giant Islander"
                CFrameQ = CFrame.new(5446.8793945313, 601.62945556641, 749.45672607422)
                CFrameMon = CFrame.new(5009.5068359375, 664.11071777344, -40.960144042969)
            elseif Lv == 1700 or Lv <= 1724 or SelectMonster == "Marine Commodore [Lv. 1700]" then -- Marine Commodore
                Ms = "Marine Commodore [Lv. 1700]"
                NameQuest = "MarineTreeIsland"
                QuestLv = 1
                NameMon = "Marine Commodore"
                CFrameQ = CFrame.new(2179.98828125, 28.731239318848, -6740.0551757813)
                CFrameMon = CFrame.new(2198.0063476563, 128.71075439453, -7109.5043945313)
            elseif Lv == 1725 or Lv <= 1774 or SelectMonster == "Marine Rear Admiral [Lv. 1725]" then -- Marine Rear Admiral
                Ms = "Marine Rear Admiral [Lv. 1725]"
                NameQuest = "MarineTreeIsland"
                QuestLv = 2
                NameMon = "Marine Rear Admiral"
                CFrameQ = CFrame.new(2179.98828125, 28.731239318848, -6740.0551757813)
                CFrameMon = CFrame.new(3294.3142089844, 385.41125488281, -7048.6342773438)
            elseif Lv == 1775 or Lv <= 1799 or SelectMonster == "Fishman Raider [Lv. 1775]" then -- Fishman Raide
                Ms = "Fishman Raider [Lv. 1775]"
                NameQuest = "DeepForestIsland3"
                QuestLv = 1
                NameMon = "Fishman Raider"
                CFrameQ = CFrame.new(-10582.759765625, 331.78845214844, -8757.666015625)
                CFrameMon = CFrame.new(-10553.268554688, 521.38439941406, -8176.9458007813)
            elseif Lv == 1800 or Lv <= 1824 or SelectMonster == "Fishman Captain [Lv. 1800]" then -- Fishman Captain
                Ms = "Fishman Captain [Lv. 1800]"
                NameQuest = "DeepForestIsland3"
                QuestLv = 2
                NameMon = "Fishman Captain"
                CFrameQ = CFrame.new(-10583.099609375, 331.78845214844, -8759.4638671875)
                CFrameMon = CFrame.new(-10789.401367188, 427.18637084961, -9131.4423828125)
            elseif Lv == 1825 or Lv <= 1849 or SelectMonster == "Forest Pirate [Lv. 1825]" then -- Forest Pirate
                Ms = "Forest Pirate [Lv. 1825]"
                NameQuest = "DeepForestIsland"
                QuestLv = 1
                NameMon = "Forest Pirate"
                CFrameQ = CFrame.new(-13232.662109375, 332.40396118164, -7626.4819335938)
                CFrameMon = CFrame.new(-13489.397460938, 400.30349731445, -7770.251953125)
            elseif Lv == 1850 or Lv <= 1899 or SelectMonster == "Mythological Pirate [Lv. 1850]" then -- Mythological Pirate
                Ms = "Mythological Pirate [Lv. 1850]"
                NameQuest = "DeepForestIsland"
                QuestLv = 2
                NameMon = "Mythological Pirate"
                CFrameQ = CFrame.new(-13232.662109375, 332.40396118164, -7626.4819335938)
                CFrameMon = CFrame.new(-13508.616210938, 582.46228027344, -6985.3037109375)
            elseif Lv == 1900 or Lv <= 1924 or SelectMonster == "Jungle Pirate [Lv. 1900]" then -- Jungle Pirate
                Ms = "Jungle Pirate [Lv. 1900]"
                NameQuest = "DeepForestIsland2"
                QuestLv = 1
                NameMon = "Jungle Pirate"
                CFrameQ = CFrame.new(-12682.096679688, 390.88653564453, -9902.1240234375)
                CFrameMon = CFrame.new(-12267.103515625, 459.75262451172, -10277.200195313)
            elseif Lv == 1925 or Lv <= 1974 or SelectMonster == "Musketeer Pirate [Lv. 1925]" then -- Musketeer Pirate
                Ms = "Musketeer Pirate [Lv. 1925]"
                NameQuest = "DeepForestIsland2"
                QuestLv = 2
                NameMon = "Musketeer Pirate"
                CFrameQ = CFrame.new(-12682.096679688, 390.88653564453, -9902.1240234375)
                CFrameMon = CFrame.new(-13291.5078125, 520.47338867188, -9904.638671875)
            elseif Lv == 1975 or Lv <= 1999 or SelectMonster == "Reborn Skeleton [Lv. 1975]" then
                Ms = "Reborn Skeleton [Lv. 1975]"
                NameQuest = "HauntedQuest1"
                QuestLv = 1
                NameMon = "Reborn Skeleton"
                CFrameQ = CFrame.new(-9480.80762, 142.130661, 5566.37305, -0.00655503059, 4.52954225e-08, -0.999978542, 2.04920472e-08, 1, 4.51620679e-08, 0.999978542, -2.01955679e-08, -0.00655503059)
                CFrameMon = CFrame.new(-8761.77148, 183.431747, 6168.33301, 0.978073597, -1.3950732e-05, -0.208259016, -1.08073925e-06, 1, -7.20630269e-05, 0.208259016, 7.07080399e-05, 0.978073597)
            elseif Lv == 2000 or Lv <= 2024 or SelectMonster == "Living Zombie [Lv. 2000]" then
                Ms = "Living Zombie [Lv. 2000]"
                NameQuest = "HauntedQuest1"
                QuestLv = 2
                NameMon = "Living Zombie"
                CFrameQ = CFrame.new(-9480.80762, 142.130661, 5566.37305, -0.00655503059, 4.52954225e-08, -0.999978542, 2.04920472e-08, 1, 4.51620679e-08, 0.999978542, -2.01955679e-08, -0.00655503059)
                CFrameMon = CFrame.new(-10103.7529, 238.565979, 6179.75977, 0.999474227, 2.77547141e-08, 0.0324240364, -2.58006327e-08, 1, -6.06848474e-08, -0.0324240364, 5.98163865e-08, 0.999474227)
            elseif Lv == 2025 or Lv <= 2049 or SelectMonster == "Demonic Soul [Lv. 2025]" then
                Ms = "Demonic Soul [Lv. 2025]"
                NameQuest = "HauntedQuest2"
                QuestLv = 1
                NameMon = "Demonic Soul"
                CFrameQ = CFrame.new(-9515.39551, 172.266037, 6078.89746, 0.0121199936, -9.78649624e-08, 0.999926567, 2.30358754e-08, 1, 9.75929382e-08, -0.999926567, 2.18513581e-08, 0.0121199936)
                CFrameMon = CFrame.new(-9709.30762, 204.695892, 6044.04688, -0.845798075, -3.4587876e-07, -0.533503294, -4.46235369e-08, 1, -5.77571257e-07, 0.533503294, -4.64701827e-07, -0.845798075)
            elseif Lv == 2050 or Lv <= 2074 or SelectMonster == "Posessed Mummy [Lv. 2050]" then
                Ms = "Posessed Mummy [Lv. 2050]"
                NameQuest = "HauntedQuest2"
                QuestLv = 2
                NameMon = "Posessed Mummy"
                CFrameQ = CFrame.new(-9515.39551, 172.266037, 6078.89746, 0.0121199936, -9.78649624e-08, 0.999926567, 2.30358754e-08, 1, 9.75929382e-08, -0.999926567, 2.18513581e-08, 0.0121199936)
                CFrameMon = CFrame.new(-9554.11035, 65.6141663, 6041.73584, -0.877069294, 5.33355795e-08, -0.480364174, 2.06420765e-08, 1, 7.33423562e-08, 0.480364174, 5.44105987e-08, -0.877069294)
            elseif Lv == 2075 or Lv <= 2099 or SelectMonster == "Peanut Scout [Lv. 2075]" then
                Ms = "Peanut Scout [Lv. 2075]"
                NameQuest ="NutsIslandQuest"
                QuestLv = 1
                NameMon = "Peanut Scout"
                POSQ = CFrame.new(-2102.74268, 38.1297836, -10192.501, 0.75739336, -4.93203451e-08, 0.65295893, 2.07778754e-08, 1, 5.14325187e-08, -0.65295893, -2.53875481e-08, 0.75739336)
                CFrameMon = CFrame.new(-1983.2562255859375, 38.12957000732422, -10588.0263671875)
            elseif Lv == 2100 or Lv <= 2124 or SelectMonster == "Peanut President [Lv. 2100]" then
                Ms = "Peanut President [Lv. 2100]"
                NameQuest ="NutsIslandQuest"
                QuestLv = 2
                NameMon = "Peanut President"
                POSQ = CFrame.new(-2102.74268, 38.1297836, -10192.501, 0.75739336, -4.93203451e-08, 0.65295893, 2.07778754e-08, 1, 5.14325187e-08, -0.65295893, -2.53875481e-08, 0.75739336)
                CFrameMon = CFrame.new(-1983.2562255859375, 38.12957000732422, -10588.0263671875)
            elseif Lv == 2125 or Lv <= 2149 or SelectMonster == "Ice Cream Chef [Lv. 2125]" then
                Ms = "Ice Cream Chef [Lv. 2125]"
                NameQuest ="IceCreamIslandQuest"
                QuestLv = 1
                NameMon = "Ice Cream Chef"
                POSQ = CFrame.new(-819.84533691406, 65.845329284668, -10965.487304688)
                CFrameMon = CFrame.new(-855.2096557617188, 65.8453598022461, -10910.7177734375)
            elseif Lv == 2150 or Lv <= 2199 or SelectMonster == "Ice Cream Commander [Lv. 2150]" then
                Ms = "Ice Cream Commander [Lv. 2150]"
                NameQuest ="IceCreamIslandQuest"
                QuestLv = 2
                NameMon = "Ice Cream Commander"
                POSQ = CFrame.new(-819.84533691406, 65.845329284668, -10965.487304688)
                CFrameMon = CFrame.new(-855.2096557617188, 65.8453598022461, -10910.7177734375)
                elseif Lv == 2200 or Lv <= 2224 or SelectMonster == "Cookie Crafter [Lv. 2200]" then
                Ms = "Cookie Crafter [Lv. 2200]"
                NameQuest = "CakeQuest1"
                QuestLv = 1
                NameMon = "Cookie Crafter"
                CFrameQ = CFrame.new(-2022.29858, 36.9275894, -12030.9766, -0.961273909, 0, -0.275594592, 0, 1, 0, 0.275594592, 0, -0.961273909)
                CFrameMon = CFrame.new(-2321.71216, 36.699482, -12216.7871, -0.780074954, 0, 0.625686109, 0, 1, 0, -0.625686109, 0, -0.780074954)
            elseif Lv == 2225 or Lv <= 2249 or SelectMonster == "Cake Guard [Lv. 2225]" then
                Ms = "Cake Guard [Lv. 2225]"
                NameQuest = "CakeQuest1"
                QuestLv = 2
                NameMon = "Cake Guard"
                CFrameQ = CFrame.new(-2022.29858, 36.9275894, -12030.9766, -0.961273909, 0, -0.275594592, 0, 1, 0, 0.275594592, 0, -0.961273909)
                CFrameMon = CFrame.new(-1418.11011, 36.6718941, -12255.7324, 0.0677844882, 0, 0.997700036, 0, 1, 0, -0.997700036, 0, 0.0677844882)
            elseif Lv == 2250 or Lv <= 2274 or SelectMonster == "Baking Staff [Lv. 2250]" then
                Ms = "Baking Staff [Lv. 2250]"
                NameQuest = "CakeQuest2"
                QuestLv = 1
                NameMon = "Baking Staff"
                CFrameQ = CFrame.new(-1928.31763, 37.7296638, -12840.626, 0.951068401, -0, -0.308980465, 0, 1, -0, 0.308980465, 0, 0.951068401)
                CFrameMon = CFrame.new(-1980.43848, 36.6716766, -12983.8418, -0.254443765, 0, -0.967087567, 0, 1, 0, 0.967087567, 0, -0.254443765)
            elseif Lv >= 2275 or SelectMonster == "Head Baker [Lv. 2275]" then
                Ms = "Head Baker [Lv. 2275]"
                NameQuest = "CakeQuest2"
                QuestLv = 2
                NameMon = "Head Baker"
                CFrameQ = CFrame.new(-1927.9891357421875, 37.97220230102539, -12841.892578125)
                CFrameMon = CFrame.new(-2307.778076171875, 105.85140228271484, -12931.0146484375)
            end
        end
    end
       function topos(Pos)
        Distance = (Pos.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
        if game.Players.LocalPlayer.Character.Humanoid.Sit == true then game.Players.LocalPlayer.Character.Humanoid.Sit = false end
        pcall(function() tween = game:GetService("TweenService"):Create(game.Players.LocalPlayer.Character.HumanoidRootPart,TweenInfo.new(Distance/210, Enum.EasingStyle.Linear),{CFrame = Pos}) end)
        tween:Play()
        if Distance <= 250 then
            tween:Cancel()
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = Pos
        end
        if _G.StopTween == true then
            tween:Cancel()
            _G.Clip = false
        end
    end
    
    function GetDistance(target)
        return math.floor((target.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude)
    end

    function TP(P1)
        Distance = (P1.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
        if Distance < 220 then
            Speed = 350
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = P1
        elseif Distance < 300 then
            Speed = 290
        elseif Distance < 500 then
            Speed = 240
        elseif Distance >= 1000 then
            Speed = 270
        end
        game:GetService("TweenService"):Create(
            game.Players.LocalPlayer.Character.HumanoidRootPart,
            TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear),
            {CFrame = P1}
        ):Play()
    end
    
    function TP2(P1)
        Distance = (P1.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
        if Distance < 220 then
            Speed = 300
            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = P1
        elseif Distance >= 1000 then
            Speed = 250
        end
        game:GetService("TweenService"):Create(
            game.Players.LocalPlayer.Character.HumanoidRootPart,
            TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear),
            {CFrame = P1}
        ):Play()
    end
    
    Old_World = false
    New_World = false
    Three_World = false
    
    local placeId = game.PlaceId
    if placeId == 2753915549 then
     Old_World = true
    elseif placeId == 4442272183 then
     New_World = true
    elseif placeId == 7449423635 then
     Three_World = true
    end
     if game.PlaceId == 2753915549 then
         World1 = true
     elseif game.PlaceId == 4442272183 then
         World2 = true
     elseif game.PlaceId == 7449423635 then
         World3 = true
     end
    
    function CheckQuest() 
        MyLevel = game:GetService("Players").LocalPlayer.Data.Level.Value
        if World1 then
            if MyLevel == 1 or MyLevel <= 9 then
                Mon = "Bandit [Lv. 5]"
                LevelQuest = 1
                NameQuest = "BanditQuest1"
                NameMon = "Bandit"
                CFrameQuest = CFrame.new(1059.37195, 15.4495068, 1550.4231, 0.939700544, -0, -0.341998369, 0, 1, -0, 0.341998369, 0, 0.939700544)
            elseif MyLevel == 10 or MyLevel <= 14 then
                Mon = "Monkey [Lv. 14]"
                LevelQuest = 1
                NameQuest = "JungleQuest"
                NameMon = "Monkey"
                CFrameQuest = CFrame.new(-1598.08911, 35.5501175, 153.377838, 0, 0, 1, 0, 1, -0, -1, 0, 0)
            elseif MyLevel == 15 or MyLevel <= 29 then
                Mon = "Gorilla [Lv. 20]"
                LevelQuest = 2
                NameQuest = "JungleQuest"
                NameMon = "Gorilla"
                CFrameQuest = CFrame.new(-1598.08911, 35.5501175, 153.377838, 0, 0, 1, 0, 1, -0, -1, 0, 0)
            elseif MyLevel == 30 or MyLevel <= 39 then
                Mon = "Pirate [Lv. 35]"
                LevelQuest = 1
                NameQuest = "BuggyQuest1"
                NameMon = "Pirate"
                CFrameQuest = CFrame.new(-1141.07483, 4.10001802, 3831.5498, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
            elseif MyLevel == 40 or MyLevel <= 59 then
                Mon = "Brute [Lv. 45]"
                LevelQuest = 2
                NameQuest = "BuggyQuest1"
                NameMon = "Brute"
                CFrameQuest = CFrame.new(-1141.07483, 4.10001802, 3831.5498, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
            elseif MyLevel == 60 or MyLevel <= 74 then
                Mon = "Desert Bandit [Lv. 60]"
                LevelQuest = 1
                NameQuest = "DesertQuest"
                NameMon = "Desert Bandit"
                CFrameQuest = CFrame.new(894.488647, 5.14000702, 4392.43359, 0.819155693, -0, -0.573571265, 0, 1, -0, 0.573571265, 0, 0.819155693)
            elseif MyLevel == 75 or MyLevel <= 89 then
                Mon = "Desert Officer [Lv. 70]"
                LevelQuest = 2
                NameQuest = "DesertQuest"
                NameMon = "Desert Officer"
                CFrameQuest = CFrame.new(894.488647, 5.14000702, 4392.43359, 0.819155693, -0, -0.573571265, 0, 1, -0, 0.573571265, 0, 0.819155693)
            elseif MyLevel == 90 or MyLevel <= 99 then
                Mon = "Snow Bandit [Lv. 90]"
                LevelQuest = 1
                NameQuest = "SnowQuest"
                NameMon = "Snow Bandit"
                CFrameQuest = CFrame.new(1389.74451, 88.1519318, -1298.90796, -0.342042685, 0, 0.939684391, 0, 1, 0, -0.939684391, 0, -0.342042685)
            elseif MyLevel == 100 or MyLevel <= 119 then
                Mon = "Snowman [Lv. 100]"
                LevelQuest = 2
                NameQuest = "SnowQuest"
                NameMon = "Snowman"
                CFrameQuest = CFrame.new(1389.74451, 88.1519318, -1298.90796, -0.342042685, 0, 0.939684391, 0, 1, 0, -0.939684391, 0, -0.342042685)
            elseif MyLevel == 120 or MyLevel <= 149 then
                Mon = "Chief Petty Officer [Lv. 120]"
                LevelQuest = 1
                NameQuest = "MarineQuest2"
                NameMon = "Chief Petty Officer"
                CFrameQuest = CFrame.new(-5039.58643, 27.3500385, 4324.68018, 0, 0, -1, 0, 1, 0, 1, 0, 0)
            elseif MyLevel == 150 or MyLevel <= 174 then
                Mon = "Sky Bandit [Lv. 150]"
                LevelQuest = 1
                NameQuest = "SkyQuest"
                NameMon = "Sky Bandit"
                CFrameQuest = CFrame.new(-4839.53027, 716.368591, -2619.44165, 0.866007268, 0, 0.500031412, 0, 1, 0, -0.500031412, 0, 0.866007268)
            elseif MyLevel == 175 or MyLevel <= 189 then
                Mon = "Dark Master [Lv. 175]"
                LevelQuest = 2
                NameQuest = "SkyQuest"
                NameMon = "Dark Master"
                CFrameQuest = CFrame.new(-4839.53027, 716.368591, -2619.44165, 0.866007268, 0, 0.500031412, 0, 1, 0, -0.500031412, 0, 0.866007268)
            elseif MyLevel == 190 or MyLevel <= 209 then
                Mon = "Prisoner [Lv. 190]"
                LevelQuest = 1
                NameQuest = "PrisonerQuest"
                NameMon = "Prisoner"
                CFrameQuest = CFrame.new(5308.93115, 1.65517521, 475.120514, -0.0894274712, -5.00292918e-09, -0.995993316, 1.60817859e-09, 1, -5.16744869e-09, 0.995993316, -2.06384709e-09, -0.0894274712)
            elseif MyLevel == 210 or MyLevel <= 249 then
                Mon = "Dangerous Prisoner [Lv. 210]"
                LevelQuest = 2
                NameQuest = "PrisonerQuest"
                NameMon = "Dangerous Prisoner"
                CFrameQuest = CFrame.new(5308.93115, 1.65517521, 475.120514, -0.0894274712, -5.00292918e-09, -0.995993316, 1.60817859e-09, 1, -5.16744869e-09, 0.995993316, -2.06384709e-09, -0.0894274712)
            elseif MyLevel == 250 or MyLevel <= 274 then
                Mon = "Toga Warrior [Lv. 250]"
                LevelQuest = 1
                NameQuest = "ColosseumQuest"
                NameMon = "Toga Warrior"
                CFrameQuest = CFrame.new(-1580.04663, 6.35000277, -2986.47534, -0.515037298, 0, -0.857167721, 0, 1, 0, 0.857167721, 0, -0.515037298)
            elseif MyLevel == 275 or MyLevel <= 299 then
                Mon = "Gladiator [Lv. 275]"
                LevelQuest = 2
                NameQuest = "ColosseumQuest"
                NameMon = "Gladiator"
                CFrameQuest = CFrame.new(-1580.04663, 6.35000277, -2986.47534, -0.515037298, 0, -0.857167721, 0, 1, 0, 0.857167721, 0, -0.515037298)
            elseif MyLevel == 300 or MyLevel <= 324 then
                Mon = "Military Soldier [Lv. 300]"
                LevelQuest = 1
                NameQuest = "MagmaQuest"
                NameMon = "Military Soldier"
                CFrameQuest = CFrame.new(-5313.37012, 10.9500084, 8515.29395, -0.499959469, 0, 0.866048813, 0, 1, 0, -0.866048813, 0, -0.499959469)
            elseif MyLevel == 325 or MyLevel <= 374 then
                Mon = "Military Spy [Lv. 325]"
                LevelQuest = 2
                NameQuest = "MagmaQuest"
                NameMon = "Military Spy"
                CFrameQuest = CFrame.new(-5313.37012, 10.9500084, 8515.29395, -0.499959469, 0, 0.866048813, 0, 1, 0, -0.866048813, 0, -0.499959469)
            elseif MyLevel == 375 or MyLevel <= 399 then
                Mon = "Fishman Warrior [Lv. 375]"
                LevelQuest = 1
                NameQuest = "FishmanQuest"
                NameMon = "Fishman Warrior"
                CFrameQuest = CFrame.new(61122.65234375, 18.497442245483, 1569.3997802734)
                if _G.AutoFarm and (CFrameQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 10000 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(61163.8515625, 11.6796875, 1819.7841796875))
                end
            elseif MyLevel == 400 or MyLevel <= 449 then
                Mon = "Fishman Commando [Lv. 400]"
                LevelQuest = 2
                NameQuest = "FishmanQuest"
                NameMon = "Fishman Commando"
                CFrameQuest = CFrame.new(61122.65234375, 18.497442245483, 1569.3997802734)
                if _G.AutoFarm and (CFrameQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 10000 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(61163.8515625, 11.6796875, 1819.7841796875))
                end
            elseif MyLevel == 450 or MyLevel <= 474 then
                Mon = "God's Guard [Lv. 450]"
                LevelQuest = 1
                NameQuest = "SkyExp1Quest"
                NameMon = "God's Guard"
                CFrameQuest = CFrame.new(-4721.88867, 843.874695, -1949.96643, 0.996191859, -0, -0.0871884301, 0, 1, -0, 0.0871884301, 0, 0.996191859)
                if _G.AutoFarm and (CFrameQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 10000 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(-4607.82275, 872.54248, -1667.55688))
                end
            elseif MyLevel == 475 or MyLevel <= 524 then
                Mon = "Shanda [Lv. 475]"
                LevelQuest = 2
                NameQuest = "SkyExp1Quest"
                NameMon = "Shanda"
                CFrameQuest = CFrame.new(-7859.09814, 5544.19043, -381.476196, -0.422592998, 0, 0.906319618, 0, 1, 0, -0.906319618, 0, -0.422592998)
                if _G.AutoFarm and (CFrameQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 10000 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(-7894.6176757813, 5547.1416015625, -380.29119873047))
                end
            elseif MyLevel == 525 or MyLevel <= 549 then
                Mon = "Royal Squad [Lv. 525]"
                LevelQuest = 1
                NameQuest = "SkyExp2Quest"
                NameMon = "Royal Squad"
                CFrameQuest = CFrame.new(-7906.81592, 5634.6626, -1411.99194, 0, 0, -1, 0, 1, 0, 1, 0, 0)
            elseif MyLevel == 550 or MyLevel <= 624 then
                Mon = "Royal Soldier [Lv. 550]"
                LevelQuest = 2
                NameQuest = "SkyExp2Quest"
                NameMon = "Royal Soldier"
                CFrameQuest = CFrame.new(-7906.81592, 5634.6626, -1411.99194, 0, 0, -1, 0, 1, 0, 1, 0, 0)
            elseif MyLevel == 625 or MyLevel <= 649 then
                Mon = "Galley Pirate [Lv. 625]"
                LevelQuest = 1
                NameQuest = "FountainQuest"
                NameMon = "Galley Pirate"
                CFrameQuest = CFrame.new(5259.81982, 37.3500175, 4050.0293, 0.087131381, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, 0.087131381)
            elseif MyLevel >= 650 then
                Mon = "Galley Captain [Lv. 650]"
                LevelQuest = 2
                NameQuest = "FountainQuest"
                NameMon = "Galley Captain"
                CFrameQuest = CFrame.new(5259.81982, 37.3500175, 4050.0293, 0.087131381, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, 0.087131381)
            end
        elseif World2 then
            if MyLevel == 700 or MyLevel <= 724 then
                Mon = "Raider [Lv. 700]"
                LevelQuest = 1
                NameQuest = "Area1Quest"
                NameMon = "Raider"
                CFrameQuest = CFrame.new(-429.543518, 71.7699966, 1836.18188, -0.22495985, 0, -0.974368095, 0, 1, 0, 0.974368095, 0, -0.22495985)
            elseif MyLevel == 725 or MyLevel <= 774 then
                Mon = "Mercenary [Lv. 725]"
                LevelQuest = 2
                NameQuest = "Area1Quest"
                NameMon = "Mercenary"
                CFrameQuest = CFrame.new(-429.543518, 71.7699966, 1836.18188, -0.22495985, 0, -0.974368095, 0, 1, 0, 0.974368095, 0, -0.22495985)
            elseif MyLevel == 775 or MyLevel <= 799 then
                Mon = "Swan Pirate [Lv. 775]"
                LevelQuest = 1
                NameQuest = "Area2Quest"
                NameMon = "Swan Pirate"
                CFrameQuest = CFrame.new(638.43811, 71.769989, 918.282898, 0.139203906, 0, 0.99026376, 0, 1, 0, -0.99026376, 0, 0.139203906)
            elseif MyLevel == 800 or MyLevel <= 874 then
                Mon = "Factory Staff [Lv. 800]"
                NameQuest = "Area2Quest"
                LevelQuest = 2
                NameMon = "Factory Staff"
                CFrameQuest = CFrame.new(632.698608, 73.1055908, 918.666321, -0.0319722369, 8.96074881e-10, -0.999488771, 1.36326533e-10, 1, 8.92172336e-10, 0.999488771, -1.07732087e-10, -0.0319722369)
            elseif MyLevel == 875 or MyLevel <= 899 then
                Mon = "Marine Lieutenant [Lv. 875]"
                LevelQuest = 1
                NameQuest = "MarineQuest3"
                NameMon = "Marine Lieutenant"
                CFrameQuest = CFrame.new(-2440.79639, 71.7140732, -3216.06812, 0.866007268, 0, 0.500031412, 0, 1, 0, -0.500031412, 0, 0.866007268)
            elseif MyLevel == 900 or MyLevel <= 949 then
                Mon = "Marine Captain [Lv. 900]"
                LevelQuest = 2
                NameQuest = "MarineQuest3"
                NameMon = "Marine Captain"
                CFrameQuest = CFrame.new(-2440.79639, 71.7140732, -3216.06812, 0.866007268, 0, 0.500031412, 0, 1, 0, -0.500031412, 0, 0.866007268)
            elseif MyLevel == 950 or MyLevel <= 974 then
                Mon = "Zombie [Lv. 950]"
                LevelQuest = 1
                NameQuest = "ZombieQuest"
                NameMon = "Zombie"
                CFrameQuest = CFrame.new(-5497.06152, 47.5923004, -795.237061, -0.29242146, 0, -0.95628953, 0, 1, 0, 0.95628953, 0, -0.29242146)
            elseif MyLevel == 975 or MyLevel <= 999 then
                Mon = "Vampire [Lv. 975]"
                LevelQuest = 2
                NameQuest = "ZombieQuest"
                NameMon = "Vampire"
                CFrameQuest = CFrame.new(-5497.06152, 47.5923004, -795.237061, -0.29242146, 0, -0.95628953, 0, 1, 0, 0.95628953, 0, -0.29242146)
            elseif MyLevel == 1000 or MyLevel <= 1049 then
                Mon = "Snow Trooper [Lv. 1000]"
                LevelQuest = 1
                NameQuest = "SnowMountainQuest"
                NameMon = "Snow Trooper"
                CFrameQuest = CFrame.new(609.858826, 400.119904, -5372.25928, -0.374604106, 0, 0.92718488, 0, 1, 0, -0.92718488, 0, -0.374604106)
            elseif MyLevel == 1050 or MyLevel <= 1099 then
                Mon = "Winter Warrior [Lv. 1050]"
                LevelQuest = 2
                NameQuest = "SnowMountainQuest"
                NameMon = "Winter Warrior"
                CFrameQuest = CFrame.new(609.858826, 400.119904, -5372.25928, -0.374604106, 0, 0.92718488, 0, 1, 0, -0.92718488, 0, -0.374604106)
            elseif MyLevel == 1100 or MyLevel <= 1124 then
                Mon = "Lab Subordinate [Lv. 1100]"
                LevelQuest = 1
                NameQuest = "IceSideQuest"
                NameMon = "Lab Subordinate"
                CFrameQuest = CFrame.new(-6064.06885, 15.2422857, -4902.97852, 0.453972578, -0, -0.891015649, 0, 1, -0, 0.891015649, 0, 0.453972578)
            elseif MyLevel == 1125 or MyLevel <= 1174 then
                Mon = "Horned Warrior [Lv. 1125]"
                LevelQuest = 2
                NameQuest = "IceSideQuest"
                NameMon = "Horned Warrior"
                CFrameQuest = CFrame.new(-6064.06885, 15.2422857, -4902.97852, 0.453972578, -0, -0.891015649, 0, 1, -0, 0.891015649, 0, 0.453972578)
            elseif MyLevel == 1175 or MyLevel <= 1199 then
                Mon = "Magma Ninja [Lv. 1175]"
                LevelQuest = 1
                NameQuest = "FireSideQuest"
                NameMon = "Magma Ninja"
                CFrameQuest = CFrame.new(-5428.03174, 15.0622921, -5299.43457, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)
            elseif MyLevel == 1200 or MyLevel <= 1249 then
                Mon = "Lava Pirate [Lv. 1200]"
                LevelQuest = 2
                NameQuest = "FireSideQuest"
                NameMon = "Lava Pirate"
                CFrameQuest = CFrame.new(-5428.03174, 15.0622921, -5299.43457, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)
            elseif MyLevel == 1250 or MyLevel <= 1274 then
                Mon = "Ship Deckhand [Lv. 1250]"
                LevelQuest = 1
                NameQuest = "ShipQuest1"
                NameMon = "Ship Deckhand"
                CFrameQuest = CFrame.new(1037.80127, 125.092171, 32911.6016)         
                if _G.AutoFarm and (CFrameQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 10000 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(923.21252441406, 126.9760055542, 32852.83203125))
                end
            elseif MyLevel == 1275 or MyLevel <= 1299 then
                Mon = "Ship Engineer [Lv. 1275]"
                LevelQuest = 2
                NameQuest = "ShipQuest1"
                NameMon = "Ship Engineer"
                CFrameQuest = CFrame.new(1037.80127, 125.092171, 32911.6016)   
                if _G.AutoFarm and (CFrameQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 10000 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(923.21252441406, 126.9760055542, 32852.83203125))
                end             
            elseif MyLevel == 1300 or MyLevel <= 1324 then
                Mon = "Ship Steward [Lv. 1300]"
                LevelQuest = 1
                NameQuest = "ShipQuest2"
                NameMon = "Ship Steward"
                CFrameQuest = CFrame.new(968.80957, 125.092171, 33244.125)         
                if _G.AutoFarm and (CFrameQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 10000 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(923.21252441406, 126.9760055542, 32852.83203125))
                end
            elseif MyLevel == 1325 or MyLevel <= 1349 then
                Mon = "Ship Officer [Lv. 1325]"
                LevelQuest = 2
                NameQuest = "ShipQuest2"
                NameMon = "Ship Officer"
                CFrameQuest = CFrame.new(968.80957, 125.092171, 33244.125)
                if _G.AutoFarm and (CFrameQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 10000 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(923.21252441406, 126.9760055542, 32852.83203125))
                end
            elseif MyLevel == 1350 or MyLevel <= 1374 then
                Mon = "Arctic Warrior [Lv. 1350]"
                LevelQuest = 1
                NameQuest = "FrostQuest"
                NameMon = "Arctic Warrior"
                CFrameQuest = CFrame.new(5667.6582, 26.7997818, -6486.08984, -0.933587909, 0, -0.358349502, 0, 1, 0, 0.358349502, 0, -0.933587909)
                if _G.AutoFarm and (CFrameQuest.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude > 10000 then
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(-6508.5581054688, 5000.034996032715, -132.83953857422))
                end
            elseif MyLevel == 1375 or MyLevel <= 1424 then
                Mon = "Snow Lurker [Lv. 1375]"
                LevelQuest = 2
                NameQuest = "FrostQuest"
                NameMon = "Snow Lurker"
                CFrameQuest = CFrame.new(5667.6582, 26.7997818, -6486.08984, -0.933587909, 0, -0.358349502, 0, 1, 0, 0.358349502, 0, -0.933587909)
            elseif MyLevel == 1425 or MyLevel <= 1449 then
                Mon = "Sea Soldier [Lv. 1425]"
                LevelQuest = 1
                NameQuest = "ForgottenQuest"
                NameMon = "Sea Soldier"
                CFrameQuest = CFrame.new(-3054.44458, 235.544281, -10142.8193, 0.990270376, -0, -0.13915664, 0, 1, -0, 0.13915664, 0, 0.990270376)
            elseif MyLevel >= 1450 then
                Mon = "Water Fighter [Lv. 1450]"
                LevelQuest = 2
                NameQuest = "ForgottenQuest"
                NameMon = "Water Fighter"
                CFrameQuest = CFrame.new(-3054.44458, 235.544281, -10142.8193, 0.990270376, -0, -0.13915664, 0, 1, -0, 0.13915664, 0, 0.990270376)
            end
        elseif World3 then
            if MyLevel == 1500 or MyLevel <= 1524 then
                Mon = "Pirate Millionaire [Lv. 1500]"
                LevelQuest = 1
                NameQuest = "PiratePortQuest"
                NameMon = "Pirate Millionaire"
                CFrameQuest = CFrame.new(-290.074677, 42.9034653, 5581.58984, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
            elseif MyLevel == 1525 or MyLevel <= 1574 then
                Mon = "Pistol Billionaire [Lv. 1525]"
                LevelQuest = 2
                NameQuest = "PiratePortQuest"
                NameMon = "Pistol Billionaire"
                CFrameQuest = CFrame.new(-290.074677, 42.9034653, 5581.58984, 0.965929627, -0, -0.258804798, 0, 1, -0, 0.258804798, 0, 0.965929627)
            elseif MyLevel == 1575 or MyLevel <= 1599 then
                Mon = "Dragon Crew Warrior [Lv. 1575]"
                LevelQuest = 1
                NameQuest = "AmazonQuest"
                NameMon = "Dragon Crew Warrior"
                CFrameQuest = CFrame.new(5832.83594, 51.6806107, -1101.51563, 0.898790359, -0, -0.438378751, 0, 1, -0, 0.438378751, 0, 0.898790359)
            elseif MyLevel == 1600 or MyLevel <= 1624 then 
                Mon = "Dragon Crew Archer [Lv. 1600]"
                NameQuest = "AmazonQuest"
                LevelQuest = 2
                NameMon = "Dragon Crew Archer"
                CFrameQuest = CFrame.new(5833.1147460938, 51.60498046875, -1103.0693359375)
            elseif MyLevel == 1625 or MyLevel <= 1649 then
                Mon = "Female Islander [Lv. 1625]"
                NameQuest = "AmazonQuest2"
                LevelQuest = 1
                NameMon = "Female Islander"
                CFrameQuest = CFrame.new(5446.8793945313, 601.62945556641, 749.45672607422)
            elseif MyLevel == 1650 or MyLevel <= 1699 then 
                Mon = "Giant Islander [Lv. 1650]"
                NameQuest = "AmazonQuest2"
                LevelQuest = 2
                NameMon = "Giant Islander"
                CFrameQuest = CFrame.new(5446.8793945313, 601.62945556641, 749.45672607422)
            elseif MyLevel == 1700 or MyLevel <= 1724 then
                Mon = "Marine Commodore [Lv. 1700]"
                LevelQuest = 1
                NameQuest = "MarineTreeIsland"
                NameMon = "Marine Commodore"
                CFrameQuest = CFrame.new(2180.54126, 27.8156815, -6741.5498, -0.965929747, 0, 0.258804798, 0, 1, 0, -0.258804798, 0, -0.965929747)
            elseif MyLevel == 1725 or MyLevel <= 1774 then
                Mon = "Marine Rear Admiral [Lv. 1725]"
                NameMon = "Marine Rear Admiral"
                NameQuest = "MarineTreeIsland"
                LevelQuest = 2
                CFrameQuest = CFrame.new(2179.98828125, 28.731239318848, -6740.0551757813)
            elseif MyLevel == 1775 or MyLevel <= 1799 then
                Mon = "Fishman Raider [Lv. 1775]"
                LevelQuest = 1
                NameQuest = "DeepForestIsland3"
                NameMon = "Fishman Raider"
                CFrameQuest = CFrame.new(-10581.6563, 330.872955, -8761.18652, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)   
            elseif MyLevel == 1800 or MyLevel <= 1824 then
                Mon = "Fishman Captain [Lv. 1800]"
                LevelQuest = 2
                NameQuest = "DeepForestIsland3"
                NameMon = "Fishman Captain"
                CFrameQuest = CFrame.new(-10581.6563, 330.872955, -8761.18652, -0.882952213, 0, 0.469463557, 0, 1, 0, -0.469463557, 0, -0.882952213)   
            elseif MyLevel == 1825 or MyLevel <= 1849 then
                Mon = "Forest Pirate [Lv. 1825]"
                LevelQuest = 1
                NameQuest = "DeepForestIsland"
                NameMon = "Forest Pirate"
                CFrameQuest = CFrame.new(-13234.04, 331.488495, -7625.40137, 0.707134247, -0, -0.707079291, 0, 1, -0, 0.707079291, 0, 0.707134247)
            elseif MyLevel == 1850 or MyLevel <= 1899 then
                Mon = "Mythological Pirate [Lv. 1850]"
                LevelQuest = 2
                NameQuest = "DeepForestIsland"
                NameMon = "Mythological Pirate"
                CFrameQuest = CFrame.new(-13234.04, 331.488495, -7625.40137, 0.707134247, -0, -0.707079291, 0, 1, -0, 0.707079291, 0, 0.707134247)   
            elseif MyLevel == 1900 or MyLevel <= 1924 then
                Mon = "Jungle Pirate [Lv. 1900]"
                LevelQuest = 1
                NameQuest = "DeepForestIsland2"
                NameMon = "Jungle Pirate"
                CFrameQuest = CFrame.new(-12680.3818, 389.971039, -9902.01953, -0.0871315002, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, -0.0871315002)
            elseif MyLevel == 1925 or MyLevel <= 1974 then
                Mon = "Musketeer Pirate [Lv. 1925]"
                LevelQuest = 2
                NameQuest = "DeepForestIsland2"
                NameMon = "Musketeer Pirate"
                CFrameQuest = CFrame.new(-12680.3818, 389.971039, -9902.01953, -0.0871315002, 0, 0.996196866, 0, 1, 0, -0.996196866, 0, -0.0871315002)
            elseif MyLevel == 1975 or MyLevel <= 1999 then
                Mon = "Reborn Skeleton [Lv. 1975]"
                LevelQuest = 1
                NameQuest = "HauntedQuest1"
                NameMon = "Reborn Skeleton"
                CFrameQuest = CFrame.new(-9479.2168, 141.215088, 5566.09277, 0, 0, 1, 0, 1, -0, -1, 0, 0)
            elseif MyLevel == 2000 or MyLevel <= 2024 then
                Mon = "Living Zombie [Lv. 2000]"
                LevelQuest = 2
                NameQuest = "HauntedQuest1"
                NameMon = "Living Zombie"
                CFrameQuest = CFrame.new(-9479.2168, 141.215088, 5566.09277, 0, 0, 1, 0, 1, -0, -1, 0, 0)
            elseif MyLevel == 2025 or MyLevel <= 2049 then
                Mon = "Demonic Soul [Lv. 2025]"
                LevelQuest = 1
                NameQuest = "HauntedQuest2"
                NameMon = "Demonic Soul"
                CFrameQuest = CFrame.new(-9516.99316, 172.017181, 6078.46533, 0, 0, -1, 0, 1, 0, 1, 0, 0) 
            elseif MyLevel == 2050 or MyLevel <= 2074 then
                Mon = "Posessed Mummy [Lv. 2050]"
                LevelQuest = 2
                NameQuest = "HauntedQuest2"
                NameMon = "Posessed Mummy"
                CFrameQuest = CFrame.new(-9516.99316, 172.017181, 6078.46533, 0, 0, -1, 0, 1, 0, 1, 0, 0)
            elseif MyLevel == 2075 or MyLevel <= 2099 then
                Mon = "Peanut Scout [Lv. 2075]"
                LevelQuest = 1
                NameQuest = "NutsIslandQuest"
                NameMon = "Peanut Scout"
                CFrameQuest = CFrame.new(-2104.3908691406, 38.104167938232, -10194.21875, 0, 0, -1, 0, 1, 0, 1, 0, 0)
            elseif MyLevel == 2100 or MyLevel <= 2124 then
                Mon = "Peanut President [Lv. 2100]"
                LevelQuest = 2
                NameQuest = "NutsIslandQuest"
                NameMon = "Peanut President"
                CFrameQuest = CFrame.new(-2104.3908691406, 38.104167938232, -10194.21875, 0, 0, -1, 0, 1, 0, 1, 0, 0)
            elseif MyLevel == 2125 or MyLevel <= 2149 then
                Mon = "Ice Cream Chef [Lv. 2125]"
                LevelQuest = 1
                NameQuest = "IceCreamIslandQuest"
                NameMon = "Ice Cream Chef"
                CFrameQuest = CFrame.new(-820.64825439453, 65.819526672363, -10965.795898438, 0, 0, -1, 0, 1, 0, 1, 0, 0)
            elseif MyLevel == 2150 or MyLevel <= 2199 then
                Mon = "Ice Cream Commander [Lv. 2150]"
                LevelQuest = 2
                NameQuest = "IceCreamIslandQuest"
                NameMon = "Ice Cream Commander"
                CFrameQuest = CFrame.new(-820.64825439453, 65.819526672363, -10965.795898438, 0, 0, -1, 0, 1, 0, 1, 0, 0)
            elseif MyLevel == 2200 or MyLevel <= 2224 then
                Mon = "Cookie Crafter [Lv. 2200]"
                LevelQuest = 1
                NameQuest = "CakeQuest1"
                NameMon = "Cookie Crafter"
                CFrameQuest = CFrame.new(-2021.32007, 37.7982254, -12028.7295, 0.957576931, -8.80302053e-08, 0.288177818, 6.9301187e-08, 1, 7.51931211e-08, -0.288177818, -5.2032135e-08, 0.957576931)
            elseif MyLevel == 2225 or MyLevel <= 2249 then
                Mon = "Cake Guard [Lv. 2225]"
                LevelQuest = 2
                NameQuest = "CakeQuest1"
                NameMon = "Cake Guard"
                CFrameQuest = CFrame.new(-2021.32007, 37.7982254, -12028.7295, 0.957576931, -8.80302053e-08, 0.288177818, 6.9301187e-08, 1, 7.51931211e-08, -0.288177818, -5.2032135e-08, 0.957576931)
            elseif MyLevel == 2250 or MyLevel <= 2274 then
                Mon = "Baking Staff [Lv. 2250]"
                LevelQuest = 1
                NameQuest = "CakeQuest2"
                NameMon = "Baking Staff"
                CFrameQuest = CFrame.new(-1927.91602, 37.7981339, -12842.5391, -0.96804446, 4.22142143e-08, 0.250778586, 4.74911062e-08, 1, 1.49904711e-08, -0.250778586, 2.64211941e-08, -0.96804446)
            elseif MyLevel >= 2275 then
                Mon = "Head Baker [Lv. 2275]"
                LevelQuest = 2
                NameQuest = "CakeQuest2"
                NameMon = "Head Baker"
                CFrameQuest = CFrame.new(-1927.91602, 37.7981339, -12842.5391, -0.96804446, 4.22142143e-08, 0.250778586, 4.74911062e-08, 1, 1.49904711e-08, -0.250778586, 2.64211941e-08, -0.96804446)
            end
        end
    end
    
       function EquipWeapon(ToolSe)
        if game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe) then
            local tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe)
            wait(1)
            game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
        end
       end
       
       Type = 1
       spawn(function()
        while wait(.1) do
            if Type == 1 then
                Farm_Mode = CFrame.new(0, 30, 0)
            elseif Type == 2 then
                Farm_Mode = CFrame.new(0, 30, 0)
            end
        end
       end)
       
       spawn(function()
        while wait(.1) do
            Type = 1
            wait(.1)
            Type = 2
            wait(.1)
        end
       end)
       
       pcall(function()
        for i,v in pairs(game:GetService("Workspace").Map.Dressrosa.Tavern:GetDescendants()) do
            if v.ClassName == "Seat" then
                v:Destroy()
            end
        end
       end)
       
       spawn(function()
        while wait() do
            if Auto_Farm then
                if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
                    MagnetActive = false
                    CheckLevel()
                    TP(CFrameQ)
                    if (CFrameQ.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 4 then
                        wait(.1)
                        CheckLevel()
                        if (CFrameQ.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 20 then
                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NameQuest, QuestLv)
                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SetSpawnPoint")
                        else
                            TP(CFrameQ)
                        end
                    end
                elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then
                    pcall(function()
                        CheckLevel()
                        if game:GetService("Workspace").Enemies:FindFirstChild(Ms) then
                            for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                                if v.Name == Ms and v:FindFirstChild("Humanoid") then
                                    if v.Humanoid.Health > 0 then
                                        repeat game:GetService("RunService").Heartbeat:wait()
                                            if game:GetService("Workspace").Enemies:FindFirstChild(Ms) then
                                                if string.find(game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestTitle.Title.Text, NameMon) then
                                                    EquipWeapon(SelectToolWeapon)
                                                    TP(v.HumanoidRootPart.CFrame * Farm_Mode)
                                                    v.HumanoidRootPart.CanCollide = false
                                                    v.HumanoidRootPart.Size = Vector3.new(60, 60, 60)
                                                    game:GetService("VirtualUser"):CaptureController()
                                                    game:GetService("VirtualUser"):Button1Down(Vector2.new(1280, 670),workspace.CurrentCamera.CFrame)
                                                    PosMon = v.HumanoidRootPart.CFrame
                                                    MagnetActive = true
                                                else
                                                    MagnetActive = false    
                                                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AbandonQuest")
                                                end
                                            else
                                                MagnetActive = false
                                                CheckLevel()
                                                TP(CFrameMon)
                                            end
                                        until not v.Parent or v.Humanoid.Health <= 0 or Auto_Farm == false or game.Players.LocalPlayer.PlayerGui.Main.Quest.Visible == false or not game:GetService("Workspace").Enemies:FindFirstChild(v.Name)
                                    end
                                end
                            end
                        else
                            MagnetActive = false
                            CheckLevel()
                            TP(CFrameMon)
                        end
                    end)
                end
            end
        end
       end)
       
       function Click()
        game:GetService'VirtualUser':CaptureController()
        game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
       end
       
       if SelectToolWeapon then
    else
        SelectToolWeapon = ""
    end
    -- Function's Farming
    Main:Toggle("Auto Farm Level",false,function(vu)
    _G.AutoFarm = vu
    loadstring(game:HttpGet("https://raw.githubusercontent.com/x2NiceXz/idk/main/idk/idk/XYzHub.lua"))()
    if _G.AutoFarm and SelectToolWeapon == "" then
        ui:Label("AutoFarm","SelectWeapon First ",2)
    else
        Auto_Farm = vu
        SelectMsster = ""
        if vu == false then
            wait(1)
            TP(game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame)
        end
    end
    end)
    Main:Toggle("Auto Superhuman",true,function(vu)
    _G.Superhuman = vu
    end)
    spawn(function()
            while wait() do wait()
                if _G.Superhuman then
                    if game.Players.LocalPlayer.Backpack:FindFirstChild("Combat") or game.Players.LocalPlayer.Character:FindFirstChild("Combat") then
                        local args = {
                            [1] = "BuyBlackLeg"
                        }
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                    end   
                    if game.Players.LocalPlayer.Character:FindFirstChild("Superhuman") or game.Players.LocalPlayer.Backpack:FindFirstChild("Superhuman") then
                        _G.SelectWeapon = "Superhuman"
                    end  
                    if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") or game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") or game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") or game.Players.LocalPlayer.Character:FindFirstChild("Electro") or game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") or game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate") or game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") or game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw") then
                        if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg").Level.Value <= 299 then
                            _G.SelectWeapon = "Black Leg"
                        end
                        if game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") and game.Players.LocalPlayer.Backpack:FindFirstChild("Electro").Level.Value <= 299 then
                            _G.SelectWeapon = "Electro"
                        end
                        if game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate").Level.Value <= 299 then
                            _G.SelectWeapon = "Fishman Karate"
                        end
                        if game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") and game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw").Level.Value <= 299 then
                            _G.SelectWeapon = "Dragon Claw"
                        end
                        if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg").Level.Value >= 300 then
                            local args = {
                                [1] = "BuyElectro"
                            }
                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                        end
                        if game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Character:FindFirstChild("Black Leg").Level.Value >= 300 then
                            local args = {
                                [1] = "BuyElectro"
                            }
                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                        end
                        if game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") and game.Players.LocalPlayer.Backpack:FindFirstChild("Electro").Level.Value >= 300 then
                            local args = {
                                [1] = "BuyFishmanKarate"
                            }
                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                        end
                        if game.Players.LocalPlayer.Character:FindFirstChild("Electro") and game.Players.LocalPlayer.Character:FindFirstChild("Electro").Level.Value >= 300 then
                            local args = {
                                [1] = "BuyFishmanKarate"
                            }
                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                        end
                        if game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate").Level.Value >= 300 then
                            local args = {
                                [1] = "BlackbeardReward",
                                [2] = "DragonClaw",
                                [3] = "1"
                            }
                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                            local args = {
                                [1] = "BlackbeardReward",
                                [2] = "DragonClaw",
                                [3] = "2"
                            }
                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args)) 
                        end
                        if game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate").Level.Value >= 300 then
                            local args = {
                                [1] = "BlackbeardReward",
                                [2] = "DragonClaw",
                                [3] = "1"
                            }
                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                            local args = {
                                [1] = "BlackbeardReward",
                                [2] = "DragonClaw",
                                [3] = "2"
                            }
                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args)) 
                        end
                        if game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") and game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw").Level.Value >= 300 then
                            local args = {
                                [1] = "BuySuperhuman"
                            }
                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                        end
                        if game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw") and game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw").Level.Value >= 300 then
                            local args = {
                                [1] = "BuySuperhuman"
                            }
                            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                        end 
                    end
                end
            end
         end)
    if Old_World or Three_World then
        Main:Toggle("Auto Second World",false, function(vu)
            _G.AutoSecondSea = vu
            StopTween(_G.AutoSecondSea)
        end)
    end
    
        spawn(function()
            while wait() do 
                if _G.AutoSecondSea then
                    pcall(function()
                        local MyLevel = game:GetService("Players").LocalPlayer.Data.Level.Value
                        if MyLevel >= 700 and World1 then
                            if game:GetService("Workspace").Map.Ice.Door.CanCollide == false and game:GetService("Workspace").Map.Ice.Door.Transparency == 1 then
                                local CFrame1 = CFrame.new(4849.29883, 5.65138149, 719.611877)
                                repeat topos(CFrame1) wait() until (CFrame1.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 or _G.AutoSecondSea == false
                                wait(1.1)
                                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("DressrosaQuestProgress","Detective")
                                wait(0.5)
                                EquipWeapon("Key")
                                repeat topos(CFrame.new(1347.7124, 37.3751602, -1325.6488)) wait() until (Vector3.new(1347.7124, 37.3751602, -1325.6488)-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 3 or _G.AutoSecondSea == false
                                wait(0.5)
                            else
                                if game:GetService("Workspace").Map.Ice.Door.CanCollide == false and game:GetService("Workspace").Map.Ice.Door.Transparency == 1 then
                                    if game:GetService("Workspace").Enemies:FindFirstChild("Ice Admiral [Lv. 700] [Boss]") then
                                        for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                                            if v.Name == "Ice Admiral [Lv. 700] [Boss]" then
                                                if not v.Humanoid.Health <= 0 then
                                                    if v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and v.Humanoid.Health > 0 then
                                                        OldCFrameSecond = v.HumanoidRootPart.CFrame
                                                        repeat task.wait()
                                                            AutoHaki()
                                                            EquipWeapon(_G.SelectWeapon)
                                                            v.HumanoidRootPart.CanCollide = false
                                                            v.Humanoid.WalkSpeed = 0
                                                            v.Head.CanCollide = false
                                                            v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                                            v.HumanoidRootPart.CFrame = OldCFrameSecond
                                                            topos(v.HumanoidRootPart.CFrame * CFrame.new(5,10,7))
                                                            game:GetService("VirtualUser"):CaptureController()
                                                            game:GetService("VirtualUser"):Button1Down(Vector2.new(1280,672))
                                                            sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
                                                        until not _G.AutoSecondSea or not v.Parent or v.Humanoid.Health <= 0
                                                    end
                                                else 
                                                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelDressrosa")
                                                end
                                            end
                                        end
                                    else
                                        if game:GetService("ReplicatedStorage"):FindFirstChild("Ice Admiral [Lv. 700] [Boss]") then
                                            topos(game:GetService("ReplicatedStorage"):FindFirstChild("Ice Admiral [Lv. 700] [Boss]").HumanoidRootPart.CFrame * CFrame.new(5,10,7))
                                        end
                                    end
                                end
                            end
                        end
                    end)
                end
            end
        end)
    if New_World then
    Main:Toggle("Auto Third Sea",false, function(vu)
            _G.AutoThirdSea = vu
            StopTween(_G.AutoThirdSea)
        end)
    end
        spawn(function()
            while wait() do
                if _G.AutoThirdSea then
                    pcall(function()
                        if game:GetService("Players").LocalPlayer.Data.Level.Value >= 1500 and World2 then
                            _G.AutoFarm = false
                            if game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ZQuestProgress","Check") == 0 then
                                topos(CFrame.new(-1926.3221435547, 12.819851875305, 1738.3092041016))
                                if (CFrame.new(-1926.3221435547, 12.819851875305, 1738.3092041016).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 10 then
                                    wait(1.5)
                                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ZQuestProgress","Begin")
                                end
                                wait(1.8)
                                if game:GetService("Workspace").Enemies:FindFirstChild("rip_indra [Lv. 1500] [Boss]") then
                                    for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
                                        if v.Name == "rip_indra [Lv. 1500] [Boss]" then
                                            OldCFrameThird = v.HumanoidRootPart.CFrame
                                            repeat task.wait()
                                                AutoHaki()
                                                EquipWeapon(_G.SelectWeapon)
                                                topos(v.HumanoidRootPart.CFrame * CFrame.new(5,10,7))
                                                v.HumanoidRootPart.CFrame = OldCFrameThird
                                                v.HumanoidRootPart.Size = Vector3.new(50,50,50)
                                                v.HumanoidRootPart.CanCollide = false
                                                v.Humanoid.WalkSpeed = 0
                                                game:GetService'VirtualUser':CaptureController()
                                                game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
                                                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelZou")
                                                sethiddenproperty(game:GetService("Players").LocalPlayer,"SimulationRadius",math.huge)
                                            until _G.AutoThirdSea == false or v.Humanoid.Health <= 0 or not v.Parent
                                        end
                                    end
                                elseif not game:GetService("Workspace").Enemies:FindFirstChild("rip_indra [Lv. 1500] [Boss]") and (CFrame.new(-26880.93359375, 22.848554611206, 473.18951416016).Position - game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 1000 then
                                    topos(CFrame.new(-26880.93359375, 22.848554611206, 473.18951416016))
                                end
                            end
                        end
                    end)
                end
            end
        end)
    Main:Toggle("Bring Mob",true,function(vu)
        Magnet = vu
    end)
    Main:Toggle("Fast Attack",true,function(velue)
    _G.FastAttack = velue
    end)
    Weapon = {}
    for i,v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetChildren()) do
        if v:IsA("Tool") then
            table.insert(Weapon ,v.Name)
        end
    end
    local SelectWeapona = Main:Dropdown("Select Weapon",Weapon,function(value)
       SelectToolWeapon = value
    end)
    Main:Button("Refase Weapon",function()
        SelectWeapona:Clear()
        for i,v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetChildren()) do  
            SelectWeapona:Add(v.Name)
        end
    end)
    
    Stats:Seperator("Stats")
    Stats:Toggle("Melee", _G.Melee, function(vu)
        _G.Melee = vu
    end)
    Stats:Toggle("Defense", _G.Defense, function(vu)
        _G.Defense = vu
    end)
    Stats:Toggle("Sword", _G.Sword, function(vu)
        _G.Sword = vu
    end)
    Stats:Toggle("Gun", _G.Gun, function(vu)
        _G.Gun = vu
    end)
    Stats:Toggle("Blox Fruit", _G.Fruit, function(vu)
        _G.Fruit = vu
    end)
    Stats:Label("Kaitan Stats")
    Stats:Toggle("Kaitan Stats",false,function(vu)
        _G.Melee = vu
        _G.Defense = vu
    end)
    
    spawn(function()
        while wait(.1) do
            if _G.Defense then
                local args = {
                    [1] = "AddPoint",
                    [2] = "Defense",
                    [3] = 1
                }
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end
        end
    end)
    
    spawn(function()
        while wait(.1) do
            if _G.Melee then
                local args = {
                    [1] = "AddPoint",
                    [2] = "Melee",
                    [3] = 1
                }
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end
        end
    end)
    
    spawn(function()  
        while wait(.1) do 
            if _G.Sword then
                local args = {
                    [1] = "AddPoint",
                    [2] = "Sword",
                    [3] = 1
                }
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end
        end
    end)
    
    spawn(function() 
        while wait() do
            if _G.Gun then
                local args = {
                    [1] = "AddPoint",
                    [2] = "Gun",
                    [3] = 1
                }
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end
        end
    end)
    
    spawn(function()
        while wait(.1) do
            if _G.Fruit then
                local args = {
                    [1] = "AddPoint",
                    [2] = "Demon Fruit",
                    [3] = 1
                }
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
            end
        end
    end)
    
    Shop:Seperator("Shop")
    Shop:Label("Abilitis",true)
    Shop:Button("Skyjump",function()
        local args = {
            [1] = "BuyHaki",
            [2] = "Geppo"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Buso Haki",function()
        local args = {
            [1] = "BuyHaki",
            [2] = "Buso"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Observation Haki",function()
        local args = {
            [1] = "KenTalk",
            [2] = "Buy"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Soru",function()
        local args = {
            [1] = "BuyHaki",
            [2] = "Soru"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Label("Fighting Style",true)
    Shop:Button("Black Leg",function()
        local args = {
            [1] = "BuyBlackLeg"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Electro",function()
        local args = {
            [1] = "BuyElectro"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Fishman Karate",function()
        local args = {
            [1] = "BuyFishmanKarate"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Dragon Claw",function()
        local args = {
            [1] = "BlackbeardReward",
            [2] = "DragonClaw",
            [3] = "2"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Superhuman",function()
        local args = {
            [1] = "BuySuperhuman"
        }
        
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Death Step",function()
        local args = {
            [1] = "BuyDeathStep"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Sharkman Karate",function()
        local args = {
            [1] = "BuySharkmanKarate",
            [2] = true
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
        local args = {
            [1] = "BuySharkmanKarate"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Electric Claw",function()
        local string_1 = "BuyElectricClaw";
        local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
        Target:InvokeServer(string_1);
    end)
    Shop:Button("Dragon Talon",function()
        local string_1 = "BuyDragonTalon";
        local bool_1 = true;
        local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
        Target:InvokeServer(string_1, bool_1);
        local string_1 = "BuyDragonTalon";
        local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
        Target:InvokeServer(string_1);
    end)
    Shop:Label("Sword",true)
    Shop:Button("Katana",function()
        local args = {
            [1] = "BuyItem",
            [2] = "Katana"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Cutlass",function()
        local args = {
            [1] = "BuyItem",
            [2] = "Cutlass"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)  
    Shop:Button("Dual Katana",function()
        local args = {
            [1] = "BuyItem",
            [2] = "Dual Katana"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Iron Mace",function()
        local args = {
            [1] = "BuyItem",
            [2] = "Iron Mace"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Triple Katana",function()
        local args = {
            [1] = "BuyItem",
            [2] = "Triple Katana"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Pipe",function()
        local args = {
            [1] = "BuyItem",
            [2] = "Pipe"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Soul Cane",function()
        local args = {
            [1] = "BuyItem",
            [2] = "Soul Cane"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Dual-Headed Blade",function()
        local args = {
            [1] = "BuyItem",
            [2] = "Dual-Headed Blade"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Bisento",function()
        local args = {
            [1] = "BuyItem",
            [2] = "Bisento"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Pole V.2",function()
        game.ReplicatedStorage.Remotes.CommF_:InvokeServer("ThunderGodTalk")
    end)
    Shop:Label("Gun",true)
    Shop:Button("Slingshot",function()
        local args = {
            [1] = "BuyItem",
            [2] = "Slingshot"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Musket",function()
        local args = {
            [1] = "BuyItem",
            [2] = "Musket"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Flintlock",function()
        local args = {
            [1] = "BuyItem",
            [2] = "Flintlock"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Refined Slingshot",function()
        local args = {
            [1] = "BuyItem",
            [2] = "Refined Slingshot"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Refined Flintlock",function()
        local args = {
            [1] = "BuyItem",
            [2] = "Refined Flintlock"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Shop:Button("Kabucha",function()
        game.ReplicatedStorage.Remotes.CommF_:InvokeServer("BlackbeardReward", "Slingshot", "2")
    end)
    
    Island:Seperator("World's")
    Island:Button("First World",function()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelMain")
    end)
    Island:Button("Second World",function()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelDressrosa")
    end)
    Island:Button("Third World",function()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelZou")
    end)
    Island:Seperator("Island")
    if Old_World then
      Island:Button("First land",function()
          TP2(CFrame.new(1042.1501464844, 16.299360275269, 1444.3442382813))
      end)
      Island:Button("Shell Town",function()
          TP2(CFrame.new(-2599.6655273438, 6.9146227836609, 2062.2216796875))
      end)
      Island:Button("Marine Ford",function()
          TP2(CFrame.new(-5081.3452148438, 85.221641540527, 4257.3588867188))
      end)
      Island:Button("Midle Town",function()
          TP2(CFrame.new(-655.97088623047, 7.878026008606, 1573.7612304688))
      end)
      Island:Button("Jungle",function()
          TP2(CFrame.new(-1499.9877929688, 22.877912521362, 353.87060546875))
      end)
      Island:Button("Pirate",function()
          TP2(CFrame.new(-1163.3889160156, 44.777843475342, 3842.8276367188))
      end)
      Island:Button("Desert",function()
          TP2(CFrame.new(954.02056884766, 6.6275520324707, 4262.611328125))
      end)
      Island:Button("Ice Land",function()
          TP2(CFrame.new(1144.5270996094, 7.3292083740234, -1164.7322998047))
      end)
      Island:Button("Colosseum",function()
          TP2(CFrame.new(-1667.5869140625, 39.385631561279, -3135.5817871094))
      end)
      Island:Button("Prison",function()
          TP2(CFrame.new(4857.6982421875, 5.6780304908752, 732.75750732422))
      end)
      Island:Button("Mob Leader",function()
          TP2(CFrame.new(-2841.9604492188, 7.3560485839844, 5318.1040039063))
      end)
      Island:Button("Magma Land",function()
          TP2(CFrame.new(-5328.8740234375, 8.6164798736572, 8427.3994140625))
      end)
      Island:Button("Water Saven",function()
          TP2(CFrame.new(3893.953125, 5.3989524841309, -1893.4851074219))
      end)
      Island:Button("FishMan Village",function()
          TP2(CFrame.new(61191.12109375, 18.497436523438, 1561.8873291016))
      end)
      Island:Button("Fountain City",function()
          TP2(CFrame.new(5244.7133789063, 38.526943206787, 4073.4987792969))
      end)
      Island:Button("Sky Island 1",function()
          TP2(CFrame.new(-4878.0415039063, 717.71246337891, -2637.7294921875))
      end)
      Island:Button("Sky Island 2",function()
          TP2(CFrame.new(-7899.6157226563, 5545.6030273438, -422.21798706055))
      end)
    
    elseif New_World then
      Island:Button("Dock",function()
          TP2(CFrame.new(-12.519311904907, 19.302536010742, 2827.853515625))
      end)
      Island:Button("Mansion",function()
          TP2(CFrame.new(-390.34829711914, 321.89730834961, 869.00506591797))
      end)
      Island:Button("Kingdom of Rose",function()
          TP2(CFrame.new(-388.29895019531, 138.35575866699, 1132.1662597656))
      end)
      Island:Button("Cafe",function()
          TP2(CFrame.new(-379.70889282227, 73.0458984375, 304.84692382813))
      end)
      Island:Button("Sunflower",function()
          TP2(CFrame.new(-1576.7171630859, 198.61849975586, 13.725157737732))
      end)
      Island:Button("Jeramy Mountain",function()
          TP2(CFrame.new(1986.3519287109, 448.95678710938, 796.70239257813))
      end)
      Island:Button("Colossuem 2",function()
          TP2(CFrame.new(-1871.8974609375, 45.820514678955, 1359.6843261719))
      end)
      Island:Button("Usopp's Island",function()
          TP2(CFrame.new(4760.4985351563, 8.3444719314575, 2849.2426757813))
      end)
      Island:Button("Factory",function()
          TP2(CFrame.new(349.53750610352, 74.446998596191, -355.62420654297))
      end)
      Island:Button("The Bridge",function()
          TP2(CFrame.new(-1860.6354980469, 88.384948730469, -1859.1593017578))
      end)
      Island:Button("Green Bit",function()
          TP2(CFrame.new(-2202.3706054688, 73.097663879395, -2819.2687988281))
      end)
      Island:Button("Graveyard",function()
          TP2(CFrame.new(-5617.5927734375, 492.22183227539, -778.3017578125))
      end)
      Island:Button("Dark Area",function()
          TP2(CFrame.new(3464.7700195313, 13.375151634216, -3368.90234375))
      end)
      Island:Button("Superhuman Mountain",function()
          TP2(CFrame.new(561.23834228516, 401.44781494141, -5297.14453125))
      end)
      Island:Button("Lava Island",function()
          TP2(CFrame.new(-5505.9633789063, 15.977565765381, -5366.6123046875))
      end)
      Island:Button("Cold IsLand",function()
          TP2(CFrame.new(-5924.716796875, 15.977565765381, -4996.427734375))
      end)
      Island:Button("Ice Castle",function()
          TP2(CFrame.new(6111.7109375, 294.41259765625, -6716.4829101563))
      end)
      Island:Button("inscription Island",function()
          TP2(CFrame.new(-5099.01171875, 98.241539001465, 2424.4035644531))
      end)
      Island:Button("Forgotten Island",function()
          TP2(CFrame.new(-3051.9514160156, 238.87203979492, -10250.807617188))
      end)
      Island:Button("Ghost Ship",function()
          game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("requestEntrance",Vector3.new(923.21252441406, 126.9760055542, 32852.83203125))
      end)
    elseif Three_World then
      Island:Button("Port Town",function()
          TP2(CFrame.new(-275.21615600586, 43.755737304688, 5451.0659179688))
      end)
    
      Island:Button("Hydra Island",function()
          TP2(CFrame.new(5541.2685546875, 668.30456542969, 195.48069763184))
      end)
    
      Island:Button("Gaint Tree",function()
          TP2(CFrame.new(2276.0859375, 25.87850189209, -6493.03125))
      end)
    
      Island:Button("Zou ISland",function()
          TP2(CFrame.new(-10034.40234375, 331.78845214844, -8319.6923828125))
      end)
    
      Island:Button("Mansion",function()
          TP2(CFrame.new(-12548.998046875, 332.40396118164, -7603.1865234375))
      end)
    
      Island:Button("Castle on the Sea",function()
          TP2(CFrame.new(-5498.0458984375, 313.79473876953, -2860.6022949219))
      end)
    
      Island:Button("Graveyard Island",function()
          TP2(CFrame.new(-9515.07324, 142.130615, 5537.58398))
      end)
    
      Island:Button("CoCoNut Island",function()
         TP2(CFrame.new(-1846.9521484375, 38.12895965576172, -10451.0908203125))
      end)
    
      Island:Button("HoCake Island 1",function()
         TP2(CFrame.new(-927.4937133789062, 58.97153091430664, -10895.5166015625))
      end)
    
      Island:Button("HoCake Island 2",function()
         TP2(CFrame.new(-1973.823486328125, 37.82403564453125, -11883.0576171875))
    end)
    end
    
    Player:Seperator("Player")
    Playerslist = {}
        
    for i,v in pairs(game:GetService("Players"):GetChildren()) do
        table.insert(Playerslist,v.Name)
    end
    
    local SelectedPly = Player:Dropdown("Select Players",Playerslist,function(value)
        _G.SelectPly = value
    end)
    
    Player:Button("Refresh Player",function()
        Playerslist = {}
        SelectedPly:Clear()
        for i,v in pairs(game:GetService("Players"):GetChildren()) do  
            SelectedPly:Add(v.Name)
        end
    end)
    Player:Label("Player's")
    Player:Toggle("Aimbot Gun",false,function(value)
        _G.Aimbot_Gun = value
    end)
    
    spawn(function()
        while task.wait() do
            if _G.Aimbot_Gun and game:GetService("Players").LocalPlayer.Character:FindFirstChild(SelectWeaponGun) then
                pcall(function()
                    game:GetService("Players").LocalPlayer.Character[SelectWeaponGun].Cooldown.Value = 0
                    local args = {
                        [1] = game:GetService("Players"):FindFirstChild(PlayerSelectAimbot).Character.HumanoidRootPart.Position,
                        [2] = game:GetSerendvice("Players"):FindFirstChild(PlayerSelectAimbot).Character.HumanoidRootPart
                    }
                    game:GetService("Players").LocalPlayer.Character[SelectWeaponGun].RemoteFunctionShoot:InvokeServer(unpack(args))
                    game:GetService'VirtualUser':CaptureController()
                    game:GetService'VirtualUser':Button1Down(Vector2.new(1280, 672))
                end)
            end
        end
    end)
    
    Player:Toggle("Aimbot Skill",false,function(value)
        _G.Aimbot_Skill = value
    end)
    
    spawn(function()
        pcall(function()
            while task.wait() do
                if _G.Aimbot_Skill and PlayerSelectAimbot ~= nil and game.Players.LocalPlayer.Character:FindFirstChildOfClass("Tool") and game.Players.LocalPlayer.Character[game.Players.LocalPlayer.Character:FindFirstChildOfClass("Tool").Name]:FindFirstChild("MousePos") then
                    local args = {
                        [1] = game:GetService("Players"):FindFirstChild(PlayerSelectAimbot).Character.HumanoidRootPart.Position
                    }
                    
                    game:GetService("Players").LocalPlayer.Character:FindFirstChild(game.Players.LocalPlayer.Character:FindFirstChildOfClass("Tool").Name).RemoteEvent:FireServer(unpack(args))
                end
            end
        end)
    end)
    Player:Toggle("Spectate Player",false,function(value)
        SpectatePlys = value
        local plr1 = game:GetService("Players").LocalPlayer.Character.Humanoid
        local plr2 = game:GetService("Players"):FindFirstChild(_G.SelectPly)
        repeat wait(.1)
            game:GetService("Workspace").Camera.CameraSubject = game:GetService("Players"):FindFirstChild(_G.SelectPly).Character.Humanoid
        until SpectatePlys == false 
        game:GetService("Workspace").Camera.CameraSubject = game:GetService("Players").LocalPlayer.Character.Humanoid
    end)
     
    spawn(function()
        while wait() do
            pcall(function()
                local MaxDistance = math.huge
                for i,v in pairs(game:GetService("Players"):GetPlayers()) do
                    if v.Name ~= game:GetService("Players").LocalPlayer.Name then
                        local Distance = v:DistanceFromCharacter(game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position)
                        if Distance < MaxDistance then
                            MaxDistance = Distance
                            PlayerSelectAimbot = v.Name
                        end
                    end
                end
            end)
        end
    end)
    Player:Toggle("Teleport To Player",false,function(value)
        _G.TeleportPly = value
    end)
    spawn(function()
        while wait() do
            if _G.TeleportPly then
                pcall(function()
                    if _G.TeleportPly then
                        repeat topos(game:GetService("Players")[_G.SelectPly].Character.HumanoidRootPart.CFrame) wait() until _G.TeleportPly == false
                    end
                    StopTween(_G.TeleportPly)
                end)
            end
        end
    end)
    
    Dungeon:Seperator("Dungeon")
    Distance = 500
    Dungeon:Toggle("Kill Arua Mob",killaura,function(value)
        if New_World or Three_World then
            RaidsArua = value
        elseif Old_World then
            Dungeon:Label("Use In New World")
        end
    end)
    Dungeon:Toggle("Auto Next Island",autonextisland,function(value)
        if New_World or Three_World then
            NextIsland = value
        elseif Old_World then
            Dungeon:Label("Use In New World & Third Sea")
        end
    end)
    Dungeon:Toggle("Auto Awakener",autoAwakener,function(value)
        if New_World or Three_World then
            Awakener = value
        elseif Old_World then
            Dungeon:Label("Use In New World & Third Sea")
        end
    end)
    spawn(function()
        while wait() do
            if Awakener and (game:GetService("Workspace")["_WorldOrigin"].Locations["l'Ã‰glise de ProphÃ©tie"].Position - game.Players.localPlayer.Character.HumanoidRootPart.Position).magnitude <= 100 then
                local string_1 = "Awakener";
                local string_2 = "Check";
                local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
                Target:InvokeServer(string_1, string_2);
                
                local string_1 = "Awakener";
                local string_2 = "Awaken";
                local Target = game:GetService("ReplicatedStorage").Remotes["CommF_"];
                Target:InvokeServer(string_1, string_2);
            end
        end
    end)
    if New_World then
    Dungeon:Button("Teleport To Dungeon",function()
        TP(CFrame.new(-6438.73535, 250.645355, -4501.50684))
    end)
    end
    if Three_World then
    Dungeon:Button("Teleport To Dungeon",function()
        TP(CFrame.new(-5013.64941, 314.843842, -2817.8042))
    end)
    end
    if New_World then
    Dungeon:Button("Awakening Room",function()
        TP(CFrame.new(266.227783, 1.39509034, 1857.00732))
    end)
    end
    if Three_World then
    Dungeon:Button("Awakening Room",function()
        TP(CFrame.new(266.227783, 1.39509034, 1857.00732))
    end)
    end
    Dungeon:Label("Auto Raides")
    RaidsSelected = selectraids or ""
    Raidslist = {}
    RaidsModule = require(game.ReplicatedStorage.Raids)
    for i,v in pairs(RaidsModule.raids) do
        table.insert(Raidslist,v)
    end
    for i,v in pairs(RaidsModule.advancedRaids) do
        table.insert(Raidslist,v)
    end
    Dungeon:Dropdown("Select Raides",Raidslist,0,function(A)
        RaidsSelected = A
    end)
    Dungeon:Toggle("Auto Raides",autoraids,function(A)
        if Old_World then
            Dungeon:Label("Raids Use In New World & Thire World")
        else
            if RaidsSelected == "" and A then
                Dungeon:Label("Select Auto Raids First")
            else
                AutoRaids = A
            end
        end
    end)
    InRaids = true
    spawn(function()
        while wait() do
            if NextIsland then
                if StatsBypassTP == "Bypassed" and UseTP and ( game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") ) then
                    if game.Players.LocalPlayer.PlayerGui.Main.Timer.Visible == false then
                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") then
                        game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame = CFrame.new(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame.x,60,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame.z)
                        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame
                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") then
                        game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame = CFrame.new(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame.x,60,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame.z)
                        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame
                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") then
                        game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame = CFrame.new(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame.x,60,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame.z)
                        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame
                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") then
                        game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame = CFrame.new(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame.x,60,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame.z)
                        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame
                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
                        game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame = CFrame.new(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame.x,60,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame.z)
                        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame
                    end
                else
                    if game.Players.LocalPlayer.PlayerGui.Main.Timer.Visible == false then
                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") then
                        game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame = CFrame.new(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame.x,60,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame.z)
                        if (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 350 then
                            Farmtween = toTarget(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").Position,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame)
                        elseif (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 350 then
                            if Farmtween then
                                Farmtween:Stop()
                            end
                            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame
                        end
                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") then
                        game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame = CFrame.new(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame.x,60,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame.z)
                        if (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 350 then
                            Farmtween = toTarget(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").Position,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame)
                        elseif (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 350 then
                            if Farmtween then
                                Farmtween:Stop()
                            end
                            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame
                        end
                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") then
                        game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame = CFrame.new(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame.x,60,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame.z)
                        
                        if (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 350 then
                            Farmtween = toTarget(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").Position,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame)
                        elseif (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 350 then
                            if Farmtween then
                                Farmtween:Stop()
                            end
                            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame
                        end
                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") then
                        game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame = CFrame.new(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame.x,60,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame.z)
                        
                        if (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 350 then
                            Farmtween = toTarget(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").Position,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame)
                        elseif (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 350 then
                            if Farmtween then
                                Farmtween:Stop()
                            end
                            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame
                        end
                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
                        game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame = CFrame.new(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame.x,60,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame.z)
                        if (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 350 then
                            Farmtween = toTarget(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").Position,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame)
                        elseif (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 350 then
                            if Farmtween then
                                Farmtween:Stop()
                            end
                            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame
                        end
                    end
                end
            end
            if RaidsArua then
                for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
                    if RaidsArua and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and (v.HumanoidRootPart.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 400 then
                        pcall(function()
                            repeat wait()
                                v.Humanoid.Health = 0
                            until not RaidsArua or v.Humanoid.Health <= 0 or not v.Parent
                        end)
                    end
                end
            end
            if AutoRaids then
                if game.Players.LocalPlayer.Backpack:FindFirstChild("Special Microchip") or game.Players.LocalPlayer.Character:FindFirstChild("Special Microchip") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
                    if game.Players.LocalPlayer.Backpack:FindFirstChild("Special Microchip") or game.Players.LocalPlayer.Character:FindFirstChild("Special Microchip") and game.Players.LocalPlayer.PlayerGui.Main.Timer.Visible == false then
                        
                        if New_World then
                            fireclickdetector(Workspace.Map.CircleIsland.RaidSummon2.Button.Main.ClickDetector)
                        elseif Three_World then
                            fireclickdetector(Workspace.Map["Boat Castle"].RaidSummon2.Button.Main.ClickDetector)
                        end
                        wait(16)
                    elseif game.Players.LocalPlayer.PlayerGui.Main.Timer.Visible == true then
                        Useraids = true
                        pcall(function()
                            repeat wait()
                                if StatsBypassTP == "Bypassed" and UseTP and ( game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") or game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") ) then
                                    if game.Players.LocalPlayer.PlayerGui.Main.Timer.Visible == false then
                                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") then
                                        game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame = CFrame.new(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame.x,60,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame.z)
                                        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame
                                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") then
                                        game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame = CFrame.new(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame.x,60,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame.z)
                                        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame
                                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") then
                                        game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame = CFrame.new(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame.x,60,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame.z)
                                        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame
                                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") then
                                        game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame = CFrame.new(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame.x,60,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame.z)
                                        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame
                                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
                                        game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame = CFrame.new(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame.x,60,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame.z)
                                        game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame
                                    end
                                else
                                    if game.Players.LocalPlayer.PlayerGui.Main.Timer.Visible == false then
                                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") then
                                        game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame = CFrame.new(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame.x,60,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame.z)
                                        if (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 350 then
                                            Farmtween = toTarget(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").Position,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame)
                                        elseif (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 350 then
                                            if Farmtween then
                                                Farmtween:Stop()
                                            end
                                            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame
                                        end
                                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") then
                                        game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame = CFrame.new(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame.x,60,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame.z)
                                        if (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 350 then
                                            Farmtween = toTarget(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").Position,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame)
                                        elseif (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 350 then
                                            if Farmtween then
                                                Farmtween:Stop()
                                            end
                                            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame
                                        end
                                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") then
                                        game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame = CFrame.new(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame.x,60,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame.z)
                                        
                                        if (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 350 then
                                            Farmtween = toTarget(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").Position,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame)
                                        elseif (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 350 then
                                            if Farmtween then
                                                Farmtween:Stop()
                                            end
                                            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame
                                        end
                                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") then
                                        game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame = CFrame.new(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame.x,60,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame.z)
                                        
                                        if (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 350 then
                                            Farmtween = toTarget(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").Position,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame)
                                        elseif (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 350 then
                                            if Farmtween then
                                                Farmtween:Stop()
                                            end
                                            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame
                                        end
                                    elseif game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
                                        game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame = CFrame.new(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame.x,60,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame.z)
                                        if (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > 350 then
                                            Farmtween = toTarget(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").Position,game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame)
                                        elseif (game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 350 then
                                            if Farmtween then
                                                Farmtween:Stop()
                                            end
                                            game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1").CFrame
                                        end
                                    end
                                end
                                for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
                                    if AutoRaids and v:FindFirstChild("Humanoid") and v:FindFirstChild("HumanoidRootPart") and (v.HumanoidRootPart.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 400 then
                                        pcall(function()
                                            repeat wait()
                                                v.HumanoidRootPart.Transparency = 0.75
                                                v.Humanoid.Health = 0
                                            until not AutoRaids or v.Humanoid.Health <= 0 or not v.Parent
                                        end)
                                    end
                                end
                            until AutoRaids == false or not game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5") or not game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4") or not game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3") or not game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2") or not game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") or game.Players.LocalPlayer.PlayerGui.Main.Timer.Visible == false
                        end)
                    end
                else
                    Useraids = false
                    local args = {
                        [1] = "RaidsNpc",
                        [2] = "Select",
                        [3] = RaidsSelected
                    }
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
                end
            end
        end
    end)
    Dungeon:Seperator("ESP")
    Dungeon:Toggle("ESP Player",espPlayerer,function(a)
        ESPPlayer = a
        UpdatePlayerChams()
    end)
    Dungeon:Toggle("ESP Chest",espchest,function(a)
        ChestESP = a
        UpdateChestChams() 
    end)
    Dungeon:Toggle("ESP Fruits",espMisc,function(a)
        MiscESP = a
        UpdateDevilChams() 
    end)
    Dungeon:Toggle("ESP Flower",espflower,function(a)
        FlowerESP = a
        UpdateFlowerChams() 
    end)
    spawn(function()
        while wait() do
            if FlowerESP then
                UpdateFlowerChams() 
            end
            if MiscESP then
                UpdateDevilChams() 
            end
            if ChestESP then
                UpdateChestChams() 
            end
            if ESPPlayer then
                UpdatePlayerChams()
            end
        end
    end)
    function isnil(thing)
        return (thing == nil)
    end
    local function round(n)
        return math.floor(tonumber(n) + 0.5)
    end
    Number = math.random(1, 1000000)
    function UpdatePlayerChams()
        for i,v in pairs(game:GetService'Players':GetChildren()) do
            pcall(function()
                if not isnil(v.Character) then
                    if ESPPlayer then
                        if not isnil(v.Character.Head) and not v.Character.Head:FindFirstChild('NameEsp'..Number) then
                            local bill = Instance.new('BillboardGui',v.Character.Head)
                            bill.Name = 'NameEsp'..Number
                            bill.ExtentsOffset = Vector3.new(0, 1, 0)
                            bill.Size = UDim2.new(1,200,1,30)
                            bill.Adornee = v.Character.Head
                            bill.AlwaysOnTop = true
                            local name = Instance.new('TextLabel',bill)
                            name.Font = "GothamBold"
                            name.FontSize = "Size14"
                            name.TextWrapped = true
                            name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude/3) ..' M')
                            name.Size = UDim2.new(1,0,1,0)
                            name.TextYAlignment = 'Top'
                            name.BackgroundTransparency = 1
                            name.TextStrokeTransparency = 0.5
                            if v.Team == game.Players.LocalPlayer.Team then
                                name.TextColor3 = Color3.new(255,255,255)
                            else
                                name.TextColor3 = Color3.new(255,255,255)
                            end
                        else
                            v.Character.Head['NameEsp'..Number].TextLabel.Text = (v.Name ..' | '.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude/3) ..' M\nHealth : ' .. round(v.Character.Humanoid.Health*100/v.Character.Humanoid.MaxHealth) .. '%')
                        end
                    else
                        if v.Character.Head:FindFirstChild('NameEsp'..Number) then
                            v.Character.Head:FindFirstChild('NameEsp'..Number):Destroy()
                        end
                    end
                end
            end)
        end
    end
    function UpdateChestChams() 
        for i,v in pairs(game.Workspace:GetChildren()) do
            pcall(function()
                if string.find(v.Name,"Chest") then
                    if ChestESP then
                        if string.find(v.Name,"Chest") then
                            if not v:FindFirstChild('NameEsp'..Number) then
                                local bill = Instance.new('BillboardGui',v)
                                bill.Name = 'NameEsp'..Number
                                bill.ExtentsOffset = Vector3.new(0, 1, 0)
                                bill.Size = UDim2.new(1,200,1,30)
                                bill.Adornee = v
                                bill.AlwaysOnTop = true
                                local name = Instance.new('TextLabel',bill)
                                name.Font = "GothamBold"
                                name.FontSize = "Size14"
                                name.TextWrapped = true
                                name.Size = UDim2.new(1,0,1,0)
                                name.TextYAlignment = 'Top'
                                name.BackgroundTransparency = 1
                                name.TextStrokeTransparency = 0.5
                                if v.Name == "Money" then
                                    name.TextColor3 = Color3.fromRGB(255, 255, 255)
                                    name.Text = ("Money" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                                end
                                if v.Name == "Gold" then
                                    name.TextColor3 = Color3.fromRGB(255, 255, 255)
                                    name.Text = ("Gold" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                                end
                                if v.Name == "Diamond" then
                                    name.TextColor3 = Color3.fromRGB(255, 255, 255)
                                    name.Text = ("Daimond" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                                end
                            else
                                v['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                            end
                        end
                    else
                        if v:FindFirstChild('NameEsp'..Number) then
                            v:FindFirstChild('NameEsp'..Number):Destroy()
                        end
                    end
                end
            end)
        end
    end
    function UpdateDevilChams() 
        for i,v in pairs(game.Workspace:GetChildren()) do
            pcall(function()
                if MiscESP then
                    if string.find(v.Name, "Fruit") then   
                        if not v.Handle:FindFirstChild('NameEsp'..Number) then
                            local bill = Instance.new('BillboardGui',v.Handle)
                            bill.Name = 'NameEsp'..Number
                            bill.ExtentsOffset = Vector3.new(0, 1, 0)
                            bill.Size = UDim2.new(1,200,1,30)
                            bill.Adornee = v.Handle
                            bill.AlwaysOnTop = true
                            local name = Instance.new('TextLabel',bill)
                            name.Font = "GothamBold"
                            name.FontSize = "Size14"
                            name.TextWrapped = true
                            name.Size = UDim2.new(1,0,1,0)
                            name.TextYAlignment = 'Top'
                            name.BackgroundTransparency = 1
                            name.TextStrokeTransparency = 0.5
                            name.TextColor3 = Color3.fromRGB(255, 255, 255)
                            name.Text = (v.Name ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude/3) ..' M')
                        else
                            v.Handle['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Handle.Position).Magnitude/3) ..' M')
                        end
                    end
                else
                    if v.Handle:FindFirstChild('NameEsp'..Number) then
                        v.Handle:FindFirstChild('NameEsp'..Number):Destroy()
                    end
                end
            end)
        end
    end
    function UpdateFlowerChams() 
        for i,v in pairs(game.Workspace:GetChildren()) do
            pcall(function()
                if v.Name == "Flower2" or v.Name == "Flower1" then
                    if FlowerESP then 
                        if not v:FindFirstChild('NameEsp'..Number) then
                            local bill = Instance.new('BillboardGui',v)
                            bill.Name = 'NameEsp'..Number
                            bill.ExtentsOffset = Vector3.new(0, 1, 0)
                            bill.Size = UDim2.new(1,200,1,30)
                            bill.Adornee = v
                            bill.AlwaysOnTop = true
                            local name = Instance.new('TextLabel',bill)
                            name.Font = "GothamBold"
                            name.FontSize = "Size14"
                            name.TextWrapped = true
                            name.Size = UDim2.new(1,0,1,0)
                            name.TextYAlignment = 'Top'
                            name.BackgroundTransparency = 1
                            name.TextStrokeTransparency = 0.5
                            name.TextColor3 = Color3.fromRGB(255, 255, 255)
                            if v.Name == "Flower1" then 
                                name.Text = ("Blue Flower" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                                name.TextColor3 = Color3.fromRGB(255, 255, 255)
                            end
                            if v.Name == "Flower2" then
                                name.Text = ("Red Flower" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                                name.TextColor3 = Color3.fromRGB(255, 255, 255)
                            end
                        else
                            v['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
                        end
                    else
                        if v:FindFirstChild('NameEsp'..Number) then
                        v:FindFirstChild('NameEsp'..Number):Destroy()
                        end
                    end
                end   
            end)
        end
    end
    
    Misc:Seperator("Server")
    Misc:Button("Rejoin",function()
    local ts = game:GetService("TeleportService")
    local p = game:GetService("Players").LocalPlayer
    ts:Teleport(game.PlaceId, p)
    end)
    local function HttpGet(url)
    return game:GetService("HttpService"):JSONDecode(htgetf(url))
    end
    Misc:Button("Server Hop",function()
    local PlaceID = game.PlaceId
    local AllIDs = {}
    local foundAnything = ""
    local actualHour = os.date("!*t").hour
    local Deleted = false
    function TPReturner()
        local Site;
        if foundAnything == "" then
            Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100'))
        else
            Site = game.HttpService:JSONDecode(game:HttpGet('https://games.roblox.com/v1/games/' .. PlaceID .. '/servers/Public?sortOrder=Asc&limit=100&cursor=' .. foundAnything))
        end
        local ID = ""
        if Site.nextPageCursor and Site.nextPageCursor ~= "null" and Site.nextPageCursor ~= nil then
            foundAnything = Site.nextPageCursor
        end
        local num = 0;
        for i,v in pairs(Site.data) do
            local Possible = true
            ID = tostring(v.id)
            if tonumber(v.maxPlayers) > tonumber(v.playing) then
                for _,Existing in pairs(AllIDs) do
                    if num ~= 0 then
                        if ID == tostring(Existing) then
                            Possible = false
                        end
                    else
                        if tonumber(actualHour) ~= tonumber(Existing) then
                            local delFile = pcall(function()
                                -- delfile("NotSameServers.json")
                                AllIDs = {}
                                table.insert(AllIDs, actualHour)
                            end)
                        end
                    end
                    num = num + 1
                end
                if Possible == true then
                    table.insert(AllIDs, ID)
                    wait()
                    pcall(function()
                        -- writefile("NotSameServers.json", game:GetService('HttpService'):JSONEncode(AllIDs))
                        wait()
                        game:GetService("TeleportService"):TeleportToPlaceInstance(PlaceID, ID, game.Players.LocalPlayer)
                    end)
                    wait(4)
                end
            end
        end
    end
    function Teleport() 
        while wait() do
            pcall(function()
                TPReturner()
                if foundAnything ~= "" then
                    TPReturner()
                end
            end)
        end
    end
    Teleport()
    end)
    Misc:Seperator("Team")
    Misc:Button("Join Pirates Team",function()
    local args = {
        [1] = "SetTeam",
        [2] = "Pirates"
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args)) 
    local args = {
        [1] = "BartiloQuestProgress"
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    local args = {
        [1] = "Buso"
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Misc:Button("Join Marines Team",function()
    local args = {
        [1] = "SetTeam",
        [2] = "Marines"
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    local args = {
        [1] = "BartiloQuestProgress"
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    local args = {
        [1] = "Buso"
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end)
    Misc:Seperator("Open Inventory")
    Misc:Button("Open Fruit Inventory",function()
    game.Players.localPlayer.PlayerGui.Main.FruitInventory.Visible = true
    end)
    Misc:Button("Open Devil Shop",function()
    local args = {
        [1] = "GetFruits"
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    game.Players.localPlayer.PlayerGui.Main.FruitShop.Visible = true
    end)
    Misc:Button("Open Inventory",function()
    local args = {
        [1] = "getInventoryWeapons"
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    game.Players.localPlayer.PlayerGui.Main.Inventory.Visible = true
    end)
    Misc:Button("Open Color Haki",function()
    game.Players.localPlayer.PlayerGui.Main.Colors.Visible = true
    end)
    Misc:Button("Open Title Name",function()
    local args = {
        [1] = "getTitles"
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    game.Players.localPlayer.PlayerGui.Main.Titles.Visible = true
    end)
    Misc:Seperator("Miscellaneous")
    Misc:Toggle("Dodge No Cooldown",false,function(Value)
    nododgecool = Value
    NoDodgeCool()
    end)
    Misc:Toggle("Soru No Cooldown",false,function(Value)
    Sorunocool = Value
    NoSoruCool()
    end)
    Misc:Toggle("Infinit Geppo",false,function(Value)
    noGeppocool = Value
    NoGeppoCool()
    end)
    Misc:Toggle("Infinit Energy",false,function()
        
    end)
    Misc:Toggle("Infinit Ability",InfAbility,function(value)
        InfAbility = value
    end)
    spawn(function()
        while wait() do
            if InfAbility then
                InfAb()
            end
        end
    end)
    function InfAb()
        if InfAbility then
            if not game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
                local inf = Instance.new("ParticleEmitter")
                inf.Acceleration = Vector3.new(0,0,0)
                inf.Archivable = true
                inf.Drag = 20
                inf.EmissionDirection = Enum.NormalId.Top
                inf.Enabled = true
                inf.Lifetime = NumberRange.new(0.2,0.2)
                inf.LightInfluence = 0
                inf.LockedToPart = true
                inf.Name = "Agility"
                inf.Rate = 500
                local numberKeypoints2 = {
                    NumberSequenceKeypoint.new(0, 0); 
                    NumberSequenceKeypoint.new(1, 4); 
                }
                inf.Size = NumberSequence.new(numberKeypoints2)
                inf.RotSpeed = NumberRange.new(999, 9999)
                inf.Rotation = NumberRange.new(0, 0)
                inf.Speed = NumberRange.new(30, 30)
                inf.SpreadAngle = Vector2.new(360,360)
                inf.Texture = "rbxassetid://243098098"
                inf.VelocityInheritance = 0
                inf.ZOffset = 2
                inf.Transparency = NumberSequence.new(0)
                inf.Color = ColorSequence.new(Color3.fromRGB(255, 199, 41),Color3.fromRGB(255 ,199, 41))
                inf.Parent = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart
            end
        else
            if game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility") then
                game.Players.LocalPlayer.Character.HumanoidRootPart:FindFirstChild("Agility"):Destroy()
            end
        end
    end
    Misc:Toggle("White Screen Mode",false, function(vu)
        _G.WhiteScren = vu
         end)
         spawn(function()
         while wait() do
          if _G.WhiteScren then
              game:GetService("RunService"):Set3dRenderingEnabled(false)
          else
              game:GetService("RunService"):Set3dRenderingEnabled(true)
          end
      end
    end)
    Misc:Toggle("Set Spawn Points",true,function(value)
        _G.AutoSetSpawn = value
    end)
    
    spawn(function()
        pcall(function()
            while wait() do
                if _G.AutoSetSpawn then
                    if game:GetService("Players").LocalPlayer.Character.Humanoid.Health > 0 then
                        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SetSpawnPoint")
                    end
                end
            end
        end)
    end)
    Misc:Button("Fps Boost",function()
    local decalsyeeted = true -- Leaving this on makes games look shitty but the fps goes up by at least 20.
    local g = game
    local w = g.Workspace
    local l = g.Lighting
    local t = w.Terrain
    t.WaterWaveSize = 0
    t.WaterWaveSpeed = 0
    t.WaterReflectance = 0
    t.WaterTransparency = 0
    l.GlobalShadows = false
    l.FogEnd = 9e9
    l.Brightness = 0
    settings().Rendering.QualityLevel = "Level01"
    for i, v in pairs(g:GetDescendants()) do
        if v:IsA("Part") or v:IsA("Union") or v:IsA("CornerWedgePart") or v:IsA("TrussPart") then 
            v.Material = "Plastic"
            v.Reflectance = 0
        elseif v:IsA("Decal") or v:IsA("Texture") and decalsyeeted then
            v.Transparency = 1
        elseif v:IsA("ParticleEmitter") or v:IsA("Trail") then
            v.Lifetime = NumberRange.new(0)
        elseif v:IsA("Explosion") then
            v.BlastPressure = 1
            v.BlastRadius = 1
        elseif v:IsA("Fire") or v:IsA("SpotLight") or v:IsA("Smoke") or v:IsA("Sparkles") then
            v.Enabled = false
        elseif v:IsA("MeshPart") then
            v.Material = "Plastic"
            v.Reflectance = 0
            v.TextureID = 10385902758728957
        end
    end
    for i, e in pairs(l:GetChildren()) do
        if e:IsA("BlurEffect") or e:IsA("SunRaysEffect") or e:IsA("ColorCorrectionEffect") or e:IsA("BloomEffect") or e:IsA("DepthOfFieldEffect") then
            e.Enabled = false
        end
    end
    end)
    Misc:Button("Redeem All Code",function()
        function UseCode(Text)
            game:GetService("ReplicatedStorage").Remotes.Redeem:InvokeServer(Text)
        end
        UseCode("UPD16")
        UseCode("2BILLION")
        UseCode("UPD15")
        UseCode("FUDD10")
        UseCode("BIGNEWS")
        UseCode("THEGREATACE")
        UseCode("SUB2GAMERROBOT_EXP1")
        UseCode("StrawHatMaine")
        UseCode("Sub2OfficialNoobie")
        UseCode("SUB2NOOBMASTER123")
        UseCode("Sub2Daigrock")
        UseCode("Axiore")
        UseCode("TantaiGaming")
        UseCode("STRAWHATMAINE") 
        UseCode("EXP_5B")
        UseCode("kittgaming")
        UseCode("Sub2Fer999")
        UseCode("Enyu_is_Pro")
        UseCode("Magicbus")
        UseCode("JCWK")
        UseCode("Starcodeheo")
        UseCode("Bluxxy")
        end)
    local LocalPlayer = game:GetService'Players'.LocalPlayer
    local originalstam = LocalPlayer.Character.Energy.Value
    function infinitestam()
    game:GetService'Players'.LocalPlayer.Character.Energy.Changed:connect(function()
        if InfinitsEnergy then
            LocalPlayer.Character.Energy.Value = originalstam
        end 
    end)
    end
    nododgecool = false
    function NoDodgeCool()
    if nododgecool then
        for i,v in next, getgc() do
            if game.Players.LocalPlayer.Character.Dodge then
                if typeof(v) == "function" and getfenv(v).script == game.Players.LocalPlayer.Character.Dodge then
                    for i2,v2 in next, getupvalues(v) do
                        if tostring(v2) == "0.4" then
                            repeat wait(.1)
                                setupvalue(v,i2,0)
                            until not nododgecool
                        end
                    end
                end
            end
        end
    end
    end
    function NoGeppoCool()
    if noGeppocool then
        for i,v in next, getgc() do
            if game.Players.LocalPlayer.Character.Geppo then
                if typeof(v) == "function" and getfenv(v).script == game.Players.LocalPlayer.Character.Geppo then
                    for i2,v2 in next, getupvalues(v) do
                        if tostring(v2) == "0" then
                            repeat wait(.1)
                                setupvalue(v,i2,0)
                            until not noGeppocool
                        end
                    end
                end
            end
        end
    end
    end
    function NoSoruCool()
    for i, v in pairs(getgc()) do
        if type(v) == "function" and getfenv(v).script == game.Players.LocalPlayer.Character:WaitForChild("Soru") then
            for i2,v2 in pairs(debug.getupvalues(v)) do
                if type(v2) == 'table' then
                    if v2.LastUse then
                        repeat wait()
                            setupvalue(v, i2, {LastAfter = 0,LastUse = 0})
                        until not Sorunocool
                    end
                end
            end
        end
    end
    end
    Misc:Seperator("Player's Mod")
    Misc:Button("Auto Quest Player",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("PlayerHunter")
    end)
    Misc:Textbox("Fake Level",true,function(value)
        game:GetService("Players").LocalPlayer.Data.Level.Value = value
    end)
    Misc:Textbox("Fake Exp",true,function(value)
        game:GetService("Players").LocalPlayer.Data.Exp.Value = value
    end)
    Misc:Textbox("Fake Beli",true,function(value)
        game:GetService("Players").LocalPlayer.Data.Beli.Value = value
    end)
    Misc:Textbox("Fake Points",true,function(value)
        game:GetService("Players").LocalPlayer.Data.Points.Value = value
    end)
    Misc:Textbox("Fake Bounty",true,function(value)
        game:GetService("Players").LocalPlayer.leaderstats["Bounty/Honor"].Value = value
    end)
    Misc:Seperator("Fruit's Sniper")
    FruitList = {
    "Bomb-Bomb",
    "Spike-Spike",
    "Chop-Chop",
    "Spring-Spring",
    "Kilo-Kilo",
    "Spin-Spin",
    "Bird: Falcon",
    "Smoke-Smoke",
    "Flame-Flame",
    "Ice-Ice",
    "Sand-Sand",
    "Dark-Dark",
    "Revive-Revive",
    "Diamond-Diamond",
    "Light-Light",
    "Love-Love",
    "Rubber-Rubber",
    "Barrier-Barrier",
    "Magma-Magma",
    "Door-Door",
    "Quake-Quake",
    "Human-Human: Buddha",
    "String-String",
    "Bird-Bird: Phoenix",
    "Rumble-Rumble",
    "Paw-Paw",
    "Gravity-Gravity",
    "Dough-Dough",
    "Venom-Venom",
    "Shadow-Shadow",
    "Control-Control",
    "Soul-Soul",
    "Dragon-Dragon"
    }
    
    _G.SelectFruit = ""
    Misc:Dropdown("Select Fruits Sniper",FruitList,function(value)
    _G.SelectFruit = value
    end)
    Misc:Toggle("Auto Buy Fruit Sniper",_G.AutoBuyFruitSniper,function(value)
    _G.AutoBuyFruitSniper = value
    end)
    Misc:Seperator("Other Fruit's")
    Misc:Dropdown("Select Fruits Eat",FruitList,function(value)
    _G.SelectFruitEat = value
    end)
    Misc:Toggle("Auto Eat Fruit",_G.AutoEatFruit,function(value)
    _G.AutoEatFruit = value
    end)
    spawn(function()
    pcall(function()
        while wait(.1) do
            if _G.AutoEatFruit then
                game:GetService("Players").LocalPlayer.Character:FindFirstChild(_G.SelectFruitEat).EatRemote:InvokeServer()
            end
        end
    end)
    end)
    spawn(function()
    pcall(function()
        while wait(.1) do
            if _G.AutoBuyFruitSniper then
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("GetFruits")
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("PurchaseRawFruit",_G.SelectFruit)
            end 
        end
    end)
    end)
    
    Misc:Toggle("Auto Random Fruit",_G.Random_Auto,function(value)
    _G.Random_Auto = value
    end)
    spawn(function()
    pcall(function()
        while wait(.1) do
            if _G.Random_Auto then
                game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Cousin","Buy")
            end 
        end
    end)
    end)
    
    Misc:Toggle("Auto Drop Fruit",_G.DropFruit,function(value)
    _G.DropFruit = value
    end)
    spawn(function()
    while wait() do
        if _G.DropFruit then
            pcall(function()
                for i,v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetChildren()) do
                    if string.find(v.Name, "Fruit") then
                        EquipWeapon(v.Name)
                        wait(.1)
                        if game:GetService("Players").LocalPlayer.PlayerGui.Main.Dialogue.Visible == true then
                            game:GetService("Players").LocalPlayer.PlayerGui.Main.Dialogue.Visible = false
                        end
                        EquipWeapon(v.Name)
                        game:GetService("Players").LocalPlayer.Character:FindFirstChild(SelectFruit).EatRemote:InvokeServer("Drop")
                    end
                end
            for i,v in pairs(game:GetService("Players").LocalPlayer.Character:GetChildren()) do
                    if string.find(v.Name, "Fruit") then
                        EquipWeapon(v.Name)
                        wait(.1)
                        if game:GetService("Players").LocalPlayer.PlayerGui.Main.Dialogue.Visible == true then
                            game:GetService("Players").LocalPlayer.PlayerGui.Main.Dialogue.Visible = false
                        end
                        EquipWeapon(v.Name)
                        game:GetService("Players").LocalPlayer.Character:FindFirstChild(SelectFruit).EatRemote:InvokeServer("Drop")
                    end
                end
            end)
        end
    end
    end)
    
    Misc:Toggle("Auto Store Fruit",_G.AutoStoreFruit,function(value)
    _G.AutoStoreFruit = value
    end)
    spawn(function()
    pcall(function()
        while wait(.1) do
            if _G.AutoStoreFruit then
                for i,v in pairs(FruitList) do
                    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit",v)
                end
            end
        end
    end)
    end)
Misc:Toggle("Bring Fruits",_G.BringFruit,function(value)
    _G.BringFruit = value
pcall(function()
        while _G.BringFruit do wait(.1)
            for i,v in pairs(game:GetService("Workspace"):GetChildren()) do
                if v:IsA("Tool") then
                    local OldCFrame = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame				
                    game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = v.Handle.CFrame * CFrame.new(0,0,8)
                    v.Handle.CFrame = game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame
                    wait(.1)
                    game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.CFrame = OldCFrame
                end
            end
        end
    end)
end)
Misc:Button("Random Fruits",function()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Cousin","Buy")
end)
