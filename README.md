spawn(function()
    game:GetService("RunService").Heartbeat:Connect(function()
        if _G.AutoFarm then
            if not game:GetService("Workspace"):FindFirstChild("LOL") then
                local LOL = Instance.new("Part")
                LOL.Name = "LOL"
                LOL.Parent = game.Workspace
                LOL.Anchored = true
                LOL.Transparency = 0
                LOL.Size = Vector3.new(20,-0.5,20)
                LOL.Material = "Neon"
            elseif game:GetService("Workspace"):FindFirstChild("LOL") then
                game.Workspace["LOL"].CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame * CFrame.new(0,-3.5,0)
            end
        else
            if game:GetService("Workspace"):FindFirstChild("LOL") then
                game:GetService("Workspace"):FindFirstChild("LOL"):Destroy()
            end
        end
    end)
end)


spawn(function()
    while wait() do
        if game.Workspace:FindFirstChild("LOL") then
            game.Workspace:FindFirstChild("LOL").Color = Color3.new(255/255,0/255,0/255)
            for i = 0,255,10 do
                wait(.1)
                if game.Workspace:FindFirstChild("LOL") then
                    game.Workspace:FindFirstChild("LOL").Color = Color3.new(255/255,i/255,0/255)
                end
            end
            for i = 255,0,-10 do
                wait(.1)
                if game.Workspace:FindFirstChild("LOL") then
                    game.Workspace:FindFirstChild("LOL").Color = Color3.new(i/255,255/255,0/255)
                end
            end
            for i = 0,255,10 do
                wait(.1)
                if game.Workspace:FindFirstChild("LOL") then
                    game.Workspace:FindFirstChild("LOL").Color = Color3.new(0/255,255/255,i/255)
                end
            end
            for i = 255,0,-10 do
                wait(.1)
                if game.Workspace:FindFirstChild("LOL") then
                    game.Workspace:FindFirstChild("LOL").Color = Color3.new(0/255,i/255,255/255)
                end
            end
            for i = 0,255,10 do
                wait(.1)
                if game.Workspace:FindFirstChild("LOL") then
                    game.Workspace:FindFirstChild("LOL").Color = Color3.new(i/255,0/255,255/255)
                end
            end
            for i = 255,0,-10 do
                wait(.1)
                if game.Workspace:FindFirstChild("LOL") then
                    game.Workspace:FindFirstChild("LOL").Color = Color3.new(255/255,0/255,i/255)
                end
            end
        end
    end
end) 


local AkaliNotif = loadstring(game:HttpGet("https://raw.githubusercontent.com/Kinlei/Dynissimo/main/Scripts/AkaliNotif.lua"))();
local Notify = AkaliNotif.Notify;



Notify({
Description = "Loading....";
Title = "By.Fun";
Duration = 5;
});

wait(3)


Notify({
Description = "Winnable! Hub";
Title = "By.Fun";
Duration = 5;
});

wait(2)
    


    Notify({
        Description = "loaded";
        Title = "By.Fun";
        Duration = 5;
        });

                    spawn(function()
                        while wait() do
                            pcall(function()
                                game:GetService("Workspace")["_WorldOrigin"].SlashHit:Destroy()
                                game:GetService("Workspace")["_WorldOrigin"].DamageCounter:Destroy()
                                game:GetService("Workspace")["_WorldOrigin"].SwordSlash:Destroy()
                            end)
                        end
                    end)


                    local ScreenGui = Instance.new("ScreenGui")
                    local Frame = Instance.new("Frame")
                    local TextLabel = Instance.new("TextLabel")
                    local TextLabel_2 = Instance.new("TextLabel")
                    
                    
                    if game.CoreGui:FindFirstChild("Loading") then
                        game.CoreGui:FindFirstChild("Loading"):Destroy()
                     end
                    
                    
                    ScreenGui.Name = "Loading"
                    ScreenGui.Parent = game.CoreGui
                    ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
                    
                    Frame.Parent = ScreenGui
                    Frame.BackgroundColor3 = Color3.fromRGB(0, 4, 49)
                    Frame.Position = UDim2.new(0.012711864, 0, 0.484662563, 0)
                    Frame.Size = UDim2.new(0, 236, 0, 81)
                    
                    TextLabel.Parent = Frame
                    TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                    TextLabel.BackgroundTransparency = 1.000
                    TextLabel.Position = UDim2.new(0.0762711838, 0, 0, 0)
                    TextLabel.Size = UDim2.new(0, 200, 0, 50)
                    TextLabel.Font = Enum.Font.SourceSansSemibold
                    TextLabel.Text = "WhiteList Synap"
                    TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
                    TextLabel.TextSize = 20.000
                    
                    TextLabel_2.Parent = Frame
                    TextLabel_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                    TextLabel_2.BackgroundTransparency = 1.000
                    TextLabel_2.Position = UDim2.new(0.0762711838, 0, 0.38271606, 0)
                    TextLabel_2.Size = UDim2.new(0, 200, 0, 50)
                    TextLabel_2.Font = Enum.Font.SourceSansSemibold
                    TextLabel_2.Text = "Loading.."
                    TextLabel_2.TextColor3 = Color3.fromRGB(255, 255, 255)
                    TextLabel_2.TextSize = 20.000
                    wait(.5)
                    TextLabel_2.Text = "Loading."
                    wait(.4)
                    TextLabel_2.Text = "Loading.."
                    wait(.3)
                    TextLabel_2.Text = "Loading..."
                    wait(.2)
                    game.CoreGui:FindFirstChild("Loading"):Destroy()
                    

function loadsc()
local vu = game:GetService("VirtualUser")
game:GetService("Players").LocalPlayer.Idled:connect(function()
   vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
   wait(1)
   vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
end)
local vu2 = game:GetService("VirtualUser")
game:GetService("Players").LocalPlayer.Idled:connect(function()
   vu2:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
   wait(1)
   vu2:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
end)
_G.SchemeColor = Color3.fromRGB(0, 89, 255)
_G.Background = Color3.fromRGB(51, 51, 51)
_G.Header = Color3.fromRGB(25,25, 25)
_G.TextColor = Color3.fromRGB(255,255,255)
local library = {
    themes = {
        original = {
            SchemeColor = _G.SchemeColor,
            Background = _G.Background,
            Header = _G.Header ,
            TextColor = _G.TextColor
        }
    }
}
local chars = 'abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789'
local length = 20
local randomString = ''
math.randomseed(os.time())
local charTable = {}
for c in chars:gmatch"." do
    table.insert(charTable, c)
end
for i = 1, length do
    randomString = randomString .. charTable[math.random(1, #charTable)]
end
for i,v in pairs(game:GetService("CoreGui"):GetChildren()) do
    if v.ClassName == "ScreenGui" then
        for i1,v1 in pairs(v:GetChildren()) do
            if v1.Name == "Main" then
                for i2,v2 in pairs(v1:GetChildren()) do
                    do
                        local ui = v
                        if ui then
                            ui:Destroy()
                        end
                    end
                end
            end
        end
    end
end

local UserInputService = game:GetService("UserInputService")
local TweenService = game:GetService("TweenService")
local RunService = game:GetService("RunService")
local LocalPlayer = game:GetService("Players").LocalPlayer
local Mouse = LocalPlayer:GetMouse()

local function MakeDraggable(topbarobject, object)
    local Dragging = nil
    local DragInput = nil
    local DragStart = nil
    local StartPosition = nil

    local function Update(input)
        local Delta = input.Position - DragStart
        local pos =
            UDim2.new(
                StartPosition.X.Scale,
                StartPosition.X.Offset + Delta.X,
                StartPosition.Y.Scale,
                StartPosition.Y.Offset + Delta.Y
            )
        object.Position = pos
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
local function RippleEffect(object)
    spawn(function()
        local Ripple = Instance.new("ImageLabel")

        Ripple.Name = "Ripple"
        Ripple.Parent = object
        Ripple.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
        Ripple.BackgroundTransparency = 1.000
        Ripple.ZIndex = 8
        Ripple.Image = "rbxassetid://2708891598"
        Ripple.ImageTransparency = 0.800
        Ripple.ScaleType = Enum.ScaleType.Fit

        Ripple.Position = UDim2.new((Mouse.X - Ripple.AbsolutePosition.X) / object.AbsoluteSize.X, 0, (Mouse.Y - Ripple.AbsolutePosition.Y) / object.AbsoluteSize.Y, 0)
        TweenService:Create(Ripple, TweenInfo.new(1, Enum.EasingStyle.Quart, Enum.EasingDirection.Out), {Position = UDim2.new(-5.5, 0, -5.5, 0), Size = UDim2.new(12, 0, 12, 0)}):Play()

        wait(0.5)
        TweenService:Create(Ripple, TweenInfo.new(1, Enum.EasingStyle.Quart, Enum.EasingDirection.Out), {ImageTransparency = 1}):Play()

        wait(1)
        Ripple:Destroy()
    end)
end

local Ui = Instance.new("ScreenGui")
Ui.Name = randomString
Ui.Parent = game.CoreGui
Ui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
UserInputService.InputBegan:Connect(function(io, p)
    if io.KeyCode == Enum.KeyCode.RightControl then
        if uitoggled == false then
            Ui.Enabled = false
            uitoggled = true
        else
            Ui.Enabled = true
            io.KeyCode = false
        end
    end
end)
if syn then
    syn.protect_gui(Ui)
end

function library:CreateWindow(title,theme,closebind)
    local tabs = {}
    local s = false
    local Main = Instance.new("Frame")
    local UICorner = Instance.new("UICorner")
    local Title = Instance.new("TextLabel")
    local MainFrame = Instance.new("Frame")
    local UICorner_2 = Instance.new("UICorner")
    local SectionBack = Instance.new("Frame")
    local UICorner_3 = Instance.new("UICorner")
    local search = Instance.new("ImageButton")
    local SearchBox = Instance.new("TextBox")
    local UICorner_25 = Instance.new("UICorner")

    Main.Name = "Main"
    Main.Parent = Ui
    Main.AnchorPoint = Vector2.new(0.5, 0.5)
    Main.BackgroundColor3 = theme.Header
    Main.BorderSizePixel = 0
    Main.Position = UDim2.new(0, 900, 0, 500)
    Main.Size = UDim2.new(0, 556, 0, 366)
    Main.ZIndex = 3

    UICorner.CornerRadius = UDim.new(0, 5)
    UICorner.Parent = Main

    Title.Name = "Title"
    Title.Parent = Main
    Title.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
    Title.BackgroundTransparency = 1.000
    Title.BorderSizePixel = 0
    Title.Position = UDim2.new(0, 13, 0, 0)
    Title.Size = UDim2.new(0, 556, 0, 19)
    Title.ZIndex = 7
    Title.Font = Enum.Font.SourceSansBold
    Title.Text = title
    Title.TextColor3 = theme.TextColor
    Title.TextSize = 20.000
    Title.TextWrapped = true
    Title.TextXAlignment = Enum.TextXAlignment.Left

    MainFrame.Name = "MainFrame"
    MainFrame.Parent = Main
    MainFrame.BackgroundColor3 = theme.Background
    MainFrame.BorderSizePixel = 0
    MainFrame.Position = UDim2.new(0, 0, 0, 19)
    MainFrame.Size = UDim2.new(0, 556, 0, 346)
    MainFrame.ZIndex = 3

    UICorner_2.CornerRadius = UDim.new(0, 5)
    UICorner_2.Parent = MainFrame

    SectionBack.Name = "SectionBack"
    SectionBack.Parent = MainFrame
    SectionBack.BackgroundColor3 = theme.Header
    SectionBack.BorderSizePixel = 0
    SectionBack.Position = UDim2.new(0, 6, 0, 35)
    SectionBack.Size = UDim2.new(0, 544, 0, 304)
    SectionBack.ZIndex = 5

    UICorner_3.CornerRadius = UDim.new(0, 3)
    UICorner_3.Parent = SectionBack
    MakeDraggable(Title,Main)
    search.Name = "search"
    search.Parent = Main
    search.BackgroundColor3 = Color3.fromRGB(198, 197, 200)
    search.BackgroundTransparency = 1.000
    search.LayoutOrder = 1
    search.Position = UDim2.new(0, 530, 0, 0)
    search.Size = UDim2.new(0, 18, 0, 19)
    search.ZIndex = 9
    search.Image = "rbxassetid://3926305904"
    search.ImageRectOffset = Vector2.new(964, 324)
    search.ImageRectSize = Vector2.new(36, 36)

    SearchBox.Name = "SearchBox"
    SearchBox.Parent = Main
    SearchBox.BackgroundColor3 = theme.Background
    SearchBox.Position = UDim2.new(0.825999975, 50, 0, 2)
    SearchBox.Size = UDim2.new(0, 0, 0, 15)
    SearchBox.ZIndex = 10
    SearchBox.BorderSizePixel = 0
    SearchBox.Font = Enum.Font.SourceSans
    SearchBox.PlaceholderColor3 = Color3.fromRGB(239, 239, 239)
    SearchBox.Text = ""
    SearchBox.TextColor3 = theme.TextColor
    SearchBox.TextSize = 14.000
    SearchBox.Visible = true
    local SearchBoxTog = false

    search.MouseButton1Click:Connect(function()
        SearchBoxTog = not SearchBoxTog
        TweenService:Create(SearchBox,TweenInfo.new(.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out),{Size = SearchBoxTog and UDim2.new(0, 71, 0, 15) or UDim2.new(0, 0, 0, 15)}):Play()
        TweenService:Create(SearchBox,TweenInfo.new(.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out),{Position = SearchBoxTog and UDim2.new(0.825999975, 0, 0, 2) or UDim2.new(0.825999975, 50, 0, 2)}):Play()
    end)

    UICorner_25.Parent = SearchBox

    local TapBar = Instance.new("ScrollingFrame")
    local UICorner_16 = Instance.new("UICorner")
    local UIListLayout_3 = Instance.new("UIListLayout")

    TapBar.Name = "TapBar"
    TapBar.Parent = Main
    TapBar.BackgroundColor3 = Color3.fromRGB(41, 41, 41)
    TapBar.BorderSizePixel = 0
    TapBar.Position = UDim2.new(0, 6, 0, 28)
    TapBar.Size = UDim2.new(0, 544, 0, 21)
    TapBar.ZIndex = 5
    TapBar.ScrollBarThickness = 2
    TapBar.CanvasSize = UDim2.new(0,0,0,0)

    UICorner_16.CornerRadius = UDim.new(0, 3)
    UICorner_16.Parent = TapBar

    UIListLayout_3.Parent = TapBar
    UIListLayout_3.FillDirection = Enum.FillDirection.Horizontal
    UIListLayout_3.SortOrder = Enum.SortOrder.LayoutOrder
    local uitoggled = false
    UserInputService.InputBegan:Connect(
        function(io, p)
            if io.KeyCode == bind then
                if uitoggled == false then
                    uitoggled = true
                    wait(.5)
                    Ui.Enabled = false
                else
                    Ui.Enabled = true
                    uitoggled = false
                end
            end
        end
    )
    function library:Notification(title,desc,button)
        for i,v in pairs(MainFrame:GetChildren())do
            if v.Name == "NotiBackFrame" then
                v:Destroy()
            end
        end
        local NotiBackFrame = Instance.new("Frame")
        local Notification = Instance.new("Frame")
        local Frame = Instance.new("Frame")
        local UICorner = Instance.new("UICorner")
        local Main = Instance.new("Frame")
        local UICorner_2 = Instance.new("UICorner")
        local Main_2 = Instance.new("Frame")
        local UICorner_3 = Instance.new("UICorner")
        local TextButton = Instance.new("TextButton")
        local UICorner_4 = Instance.new("UICorner")
        local Title = Instance.new("TextLabel")
        local UICorner_5 = Instance.new("UICorner")
        local Title_2 = Instance.new("TextLabel")
        local notifications = Instance.new("ImageButton")
        

        NotiBackFrame.Name = "NotiBackFrame"
        NotiBackFrame.Parent = MainFrame
        NotiBackFrame.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
        NotiBackFrame.BackgroundTransparency = 1
        NotiBackFrame.Position = UDim2.new(-0.000238045119, 0, -0.0562442914, 0)
        NotiBackFrame.Size = UDim2.new(0, 556, 0, 366)
        NotiBackFrame.Visible = true
        NotiBackFrame.ZIndex = 100
        TweenService:Create(
            NotiBackFrame,
            TweenInfo.new(.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out),
            {Position = UDim2.new(0, -500, -0.0562442914, 0)}
        ):Play()

        Notification.Name = "Notification"
        Notification.Parent = NotiBackFrame
        Notification.BackgroundColor3 = theme.Header
        Notification.BorderSizePixel = 0
        Notification.Position = UDim2.new(0, 83, 0, 55)
        Notification.Size = UDim2.new(0, 390, 0, 255)
        Notification.ZIndex = 10
        Notification.ClipsDescendants = true

        Frame.Parent = Notification
        Frame.BackgroundColor3 = theme.Background
        Frame.BorderColor3 = Color3.fromRGB(27, 42, 53)
        Frame.BorderSizePixel = 0
        Frame.Position = UDim2.new(0, 0, 0, 17)
        Frame.Size = UDim2.new(0, 390, 0, 236)
        Frame.ZIndex = 11
        
        UICorner.CornerRadius = UDim.new(0, 5)
        UICorner.Parent = Frame
        
        Main.Name = "Main"
        Main.Parent = Frame
        Main.BackgroundColor3 = theme.Header
        Main.BorderColor3 = Color3.fromRGB(27, 42, 53)
        Main.BorderSizePixel = 0
        Main.Position = UDim2.new(0, 8, 0, 7)
        Main.Size = UDim2.new(0, 373, 0, 220)
        Main.ZIndex = 11
        
        UICorner_2.CornerRadius = UDim.new(0, 5)
        UICorner_2.Parent = Main
        
        Main_2.Name = "Main"
        Main_2.Parent = Main
        Main_2.BackgroundColor3 = theme.Background
        Main_2.BorderColor3 = Color3.fromRGB(27, 42, 53)
        Main_2.BorderSizePixel = 0
        Main_2.Position = UDim2.new(0, 6, 0, 5)
        Main_2.Size = UDim2.new(0, 360, 0, 209)
        Main_2.ZIndex = 11
        
        UICorner_3.CornerRadius = UDim.new(0, 5)
        UICorner_3.Parent = Main_2
        
        TextButton.Parent = Main_2
        TextButton.BackgroundColor3 = theme.Header
        TextButton.Position = UDim2.new(0, 13, 0, 162)
        TextButton.Size = UDim2.new(0, 335, 0, 31)
        TextButton.ZIndex = 11
        TextButton.Font = Enum.Font.SourceSansBold
        TextButton.Text = button
        TextButton.TextColor3 = theme.TextColor
        TextButton.TextSize = 20.000
        
        UICorner_4.CornerRadius = UDim.new(0, 5)
        UICorner_4.Parent = TextButton
        TextButton.MouseButton1Click:Connect(function()

            NotiBackFrame:Destroy()

        end)
        Title.Name = "Title"
        Title.Parent = Main_2
        Title.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
        Title.BackgroundTransparency = 1.000
        Title.BorderSizePixel = 0
        Title.Position = UDim2.new(0, 14, 0, 8)
        Title.Size = UDim2.new(0, 335, 0, 113)
        Title.ZIndex = 11
        Title.Font = Enum.Font.SourceSansBold
        Title.Text = desc
        Title.TextColor3 = theme.TextColor
        Title.TextSize = 20.000
        Title.TextXAlignment = Enum.TextXAlignment.Left
        Title.TextYAlignment = Enum.TextYAlignment.Top
        
        UICorner_5.CornerRadius = UDim.new(0, 5)
        UICorner_5.Parent = Notification
        
        Title_2.Name = "Title"
        Title_2.Parent = Notification
        Title_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
        Title_2.BackgroundTransparency = 1.000
        Title_2.Position = UDim2.new(0, 28, 0, 1)
        Title_2.Size = UDim2.new(0, 191, 0, 19)
        Title_2.ZIndex = 10
        Title_2.Font = Enum.Font.SourceSansBold
        Title_2.Text = title
        Title_2.TextColor3 = theme.TextColor
        Title_2.TextSize = 20.000
        Title_2.TextXAlignment = Enum.TextXAlignment.Left
        
        notifications.Name = "notifications"
        notifications.Parent = Notification
        notifications.BackgroundTransparency = 1.000
        notifications.LayoutOrder = 1
        notifications.Position = UDim2.new(0, 7, 0, 0)
        notifications.Size = UDim2.new(0, 21, 0, 20)
        notifications.ZIndex = 11
        notifications.Image = "rbxassetid://3926305904"
        notifications.ImageRectOffset = Vector2.new(844, 564)
        notifications.ImageRectSize = Vector2.new(36, 36)
    end
    function tabs:CreateTab(title)
        local SectionContent = {}
        local Tab1 = Instance.new("TextButton")
        local UICorner_17 = Instance.new("UICorner")

        Tab1.Name = "Tab"
        Tab1.Parent = TapBar
        Tab1.BackgroundColor3 = theme.Header
        Tab1.Size = UDim2.new(0, 84, 0, 20)
        Tab1.ZIndex = 6
        Tab1.Font = Enum.Font.SourceSansBold
        Tab1.Text = title
        Tab1.TextColor3 = theme.TextColor
        Tab1.TextSize = 18.000
        Tab1.TextStrokeColor3 = Color3.fromRGB(255, 255, 255)
        Tab1.TextWrapped = true

        UICorner_17.CornerRadius = UDim.new(0, 3)
        UICorner_17.Parent = Tab1

        local ScrollingFrame = Instance.new("ScrollingFrame")
        local Left = Instance.new("Frame")
        local UIListLayout_2 = Instance.new("UIListLayout")
        local Right = Instance.new("Frame")
        local UIPadding_2 = Instance.new("UIPadding")

        ScrollingFrame.Parent = SectionBack
        ScrollingFrame.Active = true
        ScrollingFrame.BackgroundColor3 = theme.Header
        ScrollingFrame.BackgroundTransparency = 1.000
        ScrollingFrame.Position = UDim2.new(0, 0, 0.0197368413, 0)
        ScrollingFrame.Size = UDim2.new(0, 542, 0, 298)
        ScrollingFrame.ScrollBarThickness = 0
        ScrollingFrame.Visible = false
        Left.Name = "Left"
        Left.Parent = ScrollingFrame
        Left.BackgroundColor3 = Color3.fromRGB(63, 63, 63)
        Left.BackgroundTransparency = 1.000
        Left.BorderSizePixel = 0
        Left.Position = UDim2.new(0, 7, 0, 5)
        Left.Size = UDim2.new(0, 262, 0, 299)
        Left.ZIndex = 6

        UIListLayout_2.Parent = ScrollingFrame
        UIListLayout_2.FillDirection = Enum.FillDirection.Horizontal
        UIListLayout_2.SortOrder = Enum.SortOrder.LayoutOrder
        UIListLayout_2.Padding = UDim.new(0, 10)
        Right.Name = "Right"
        Right.Parent = ScrollingFrame
        Right.BackgroundColor3 = Color3.fromRGB(63, 63, 63)
        Right.BackgroundTransparency = 1.000
        Right.BorderSizePixel = 0
        Right.Position = UDim2.new(0, 7, 0, 5)
        Right.Size = UDim2.new(0, 262, 0, 299)
        Right.ZIndex = 6
        local RightList = Instance.new("UIListLayout")
        local LeftList = Instance.new("UIListLayout")
        LeftList.Parent = Left
        LeftList.SortOrder = Enum.SortOrder.LayoutOrder
        LeftList.Padding = UDim.new(0, 5)
        RightList.Parent = Right
        RightList.SortOrder = Enum.SortOrder.LayoutOrder
        RightList.Padding = UDim.new(0, 5)

        TapBar.CanvasSize = UDim2.new(0,UIListLayout_3.AbsoluteContentSize.X,0,0)

        UIPadding_2.Parent = ScrollingFrame
        UIPadding_2.PaddingLeft = UDim.new(0, 5)
        if s == false then
            s = true
            Tab1.TextColor3 = theme.TextColor
            ScrollingFrame.Visible = true
            Tab1.BackgroundColor3 = theme.SchemeColor
        end

        local function GetSide(Longest)
            if Longest then
                if LeftList.AbsoluteContentSize.Y > RightList.AbsoluteContentSize.Y then
                    return Left
                else
                    return Right
                end
            else
                if LeftList.AbsoluteContentSize.Y > RightList.AbsoluteContentSize.Y then
                    return Right
                else
                    return Left
                end
            end
        end

        LeftList:GetPropertyChangedSignal("AbsoluteContentSize"):Connect(function()
            if GetSide(true).Name == Left.Name then
                ScrollingFrame.CanvasSize = UDim2.new(0,0,0,LeftList.AbsoluteContentSize.Y + 5)
            else
                ScrollingFrame.CanvasSize = UDim2.new(0,0,0,RightList.AbsoluteContentSize.Y + 5)
            end
        end)
        RightList:GetPropertyChangedSignal("AbsoluteContentSize"):Connect(function()
            if GetSide(true).Name == Left.Name then
                ScrollingFrame.CanvasSize = UDim2.new(0,0,0,LeftList.AbsoluteContentSize.Y + 5)
            else
                ScrollingFrame.CanvasSize = UDim2.new(0,0,0,RightList.AbsoluteContentSize.Y + 5)
            end
        end)
        Tab1.MouseButton1Click:Connect(function()
            for i, v in next, SectionBack:GetChildren() do
                if v.Name == "ScrollingFrame" then
                    v.Visible = false
                end
                ScrollingFrame.Visible = true

            end
            for i, v in next, TapBar:GetChildren() do
                if v.Name == "Tab" then
                    TweenService:Create(
                        v,
                        TweenInfo.new(.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out),
                        {TextColor3 = theme.TextColor}
                    ):Play()
                    TweenService:Create(
                        v,
                        TweenInfo.new(.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out),
                        {BackgroundColor3 = theme.Header}
                    ):Play()
                    TweenService:Create(
                        Tab1,
                        TweenInfo.new(.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out),
                        {TextColor3 = theme.TextColor}
                    ):Play()
                    TweenService:Create(
                        Tab1,
                        TweenInfo.new(.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out),
                        {BackgroundColor3 = theme.SchemeColor}
                    ):Play()
                end
            end
        end)



        function SectionContent:CreateSection(title)
            local Content = {}
            local SectionHold = Instance.new("Frame")
            local UICorner_4 = Instance.new("UICorner")
            local UIListLayout = Instance.new("UIListLayout")
            local UIPadding = Instance.new("UIPadding")
            SectionHold.Name = "SectionHold"
            SectionHold.Parent = GetSide(false)
            SectionHold.BackgroundColor3 = theme.Background
            SectionHold.Position = UDim2.new(0, 1, 0, 0)
            SectionHold.Size = UDim2.new(0, 260, 0, 100)
            SectionHold.ZIndex = 7

            UICorner_4.CornerRadius = UDim.new(0, 5)
            UICorner_4.Parent = SectionHold


            UIListLayout.Parent = SectionHold
            UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder
            UIListLayout.Padding = UDim.new(0, 5)
            UIListLayout:GetPropertyChangedSignal("AbsoluteContentSize"):Connect(function()
                SectionHold.Size = UDim2.new(1,0,0,UIListLayout.AbsoluteContentSize.Y + 15)
            end)
            UIPadding.Parent = SectionHold
            UIPadding.PaddingLeft = UDim.new(0, 10)
            local Title_10 = Instance.new("TextLabel")

            Title_10.Name = "Title"
            Title_10.Parent = SectionHold
            Title_10.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
            Title_10.BackgroundTransparency = 1.000
            Title_10.Position = UDim2.new(0.0449448675, 0, -0.00182170793, 0)
            Title_10.Size = UDim2.new(0, 211, 0, 31)
            Title_10.ZIndex = 8
            Title_10.Font = Enum.Font.SourceSansBold
            Title_10.Text = title
            Title_10.TextColor3 = theme.TextColor
            Title_10.TextSize = 20.000
            Title_10.TextXAlignment = Enum.TextXAlignment.Left
            
            function Content:CreateLine()
                local Line = Instance.new("Frame")
                local Frame_3 = Instance.new("Frame")
                local UICorner_8 = Instance.new('UICorner')

                Line.Name = "Line"
                Line.Parent = SectionHold
                Line.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                Line.BackgroundTransparency = 1.000
                Line.BorderSizePixel = 0
                Line.Position = UDim2.new(0, 0, 0, 71)
                Line.Size = UDim2.new(0, 224, 0, 10)
                Line.ZIndex = 7

                Frame_3.Parent = Line
                Frame_3.BackgroundColor3 = Color3.fromRGB(37, 37, 37)
                Frame_3.BorderColor3 = Color3.fromRGB(255, 255, 255)
                Frame_3.BorderSizePixel = 0
                Frame_3.Position = UDim2.new(0, 10, 0, 5)
                Frame_3.Size = UDim2.new(0, 215, 0, 5)
                Frame_3.ZIndex = 7
                UICorner_8.CornerRadius = UDim.new(0, 10)
                UICorner_8.Parent = Frame_3
            end

            function Content:CreateLabel(title)
                local LabelFunc = {}
                local Label2 = Instance.new("Frame")
                local Title_4 = Instance.new("TextLabel")
                
                Label2.Name = title
                Label2.Parent = SectionHold
                Label2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                Label2.BackgroundTransparency = 1.000
                Label2.BorderSizePixel = 0
                Label2.Position = UDim2.new(0, -11, 0, 191)
                Label2.Size = UDim2.new(0, 261, 0, 22)
                Label2.ZIndex = 7
                
                Title_4.Name = "Title"
                Title_4.Parent = Label2
                Title_4.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                Title_4.BackgroundTransparency = 1.000
                Title_4.Position = UDim2.new(0, 12, 0, -6)
                Title_4.Size = UDim2.new(0, 211, 0, 31)
                Title_4.ZIndex = 8
                Title_4.Text = title
                Title_4.Font = Enum.Font.SourceSansBold
                Title_4.TextColor3 = theme.TextColor
                Title_4.TextSize = 20.000
                function LabelFunc:Update(text)
                    Label2.Name = tostring(text)

                    Title_4.Text = tostring(text)
                end
                return LabelFunc
            end
            function Content:CreateLabel2(title)
                local LabelFunc = {}
                local Label1 = Instance.new("Frame")
                local Frame_8 = Instance.new("Frame")
                local UICorner_14 = Instance.new("UICorner")
                local Frame_9 = Instance.new("Frame")
                local UICorner_15 = Instance.new("UICorner")
                local Title_9 = Instance.new("TextLabel")
                
                Label1.Name = title
                Label1.Parent = SectionHold
                Label1.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                Label1.BackgroundTransparency = 1.000
                Label1.BorderSizePixel = 0
                Label1.Position = UDim2.new(0, 0, 0, 30)
                Label1.Size = UDim2.new(0, 260, 0, 22)
                Label1.ZIndex = 7
                
                Frame_8.Parent = Label1
                Frame_8.BackgroundColor3 = Color3.fromRGB(37, 37, 37)
                Frame_8.BorderColor3 = Color3.fromRGB(255, 255, 255)
                Frame_8.BorderSizePixel = 0
                Frame_8.Position = UDim2.new(0, 24, 0, 7)
                Frame_8.Size = UDim2.new(0, 62, 0, 4)
                Frame_8.ZIndex = 7
                
                UICorner_14.CornerRadius = UDim.new(0, 10)
                UICorner_14.Parent = Frame_8
                
                Frame_9.Parent = Label1
                Frame_9.BackgroundColor3 = Color3.fromRGB(37, 37, 37)
                Frame_9.BorderColor3 = Color3.fromRGB(255, 255, 255)
                Frame_9.BorderSizePixel = 0
                Frame_9.Position = UDim2.new(0, 156, 0, 7)
                Frame_9.Size = UDim2.new(0, 62, 0, 4)
                Frame_9.ZIndex = 7
                
                UICorner_15.CornerRadius = UDim.new(0, 10)
                UICorner_15.Parent = Frame_9
                
                Title_9.Name = "Title"
                Title_9.Parent = Label1
                Title_9.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                Title_9.BackgroundTransparency = 1.000
                Title_9.Position = UDim2.new(0, 14, 0, -7)
                Title_9.Size = UDim2.new(0, 211, 0, 31)
                Title_9.ZIndex = 8
                Title_9.Text = title
                Title_9.Font = Enum.Font.SourceSansBold
                Title_9.TextColor3 = theme.TextColor
                Title_9.TextSize = 20.000
                function LabelFunc:Update(text)
                    Label1.Name = tostring(text)
                    Title_4.Text = tostring(text)
                end
                return LabelFunc
            end
            local focused = false
            SearchBox.Focused:Connect(function()
            
            end)
            SearchBox.FocusLost:Connect(function()
            
            end)

            function UpdateInputOfSearchText()
                local InputText = string.upper(SearchBox.Text)
                for _,button in pairs(SectionHold:GetChildren())do
                    if button:IsA("Frame") then
                                if InputText == "" or string.find(string.upper(button.Name),InputText) ~= nil then
                                    button.Visible = true
                                else
                                    button.Visible = false
                                end
                    end
                end
            end

            SearchBox.Changed:Connect(UpdateInputOfSearchText)
            function Content:CreateButton(title,callback)
                local Button = Instance.new("Frame")
                local TextButton = Instance.new("TextButton")
                local UICorner_5 = Instance.new("UICorner")
                local touch_app = Instance.new("ImageButton")

                Button.Name = title
                Button.Parent = SectionHold
                Button.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                Button.BackgroundTransparency = 1.000
                Button.BorderSizePixel = 0
                Button.ClipsDescendants = true
                Button.Position = UDim2.new(0, 0, 0, 87)
                Button.Size = UDim2.new(0, 240, 0, 34)
                Button.ZIndex = 8

                TextButton.Parent = Button
                TextButton.BackgroundColor3 = theme.Header
                TextButton.BorderSizePixel = 0
                TextButton.Position = UDim2.new(0, 12, 0, 5)
                TextButton.Size = UDim2.new(0, 212, 0, 26)
                TextButton.ZIndex = 7
                TextButton.Font = Enum.Font.SourceSansBold
                TextButton.TextColor3 = theme.TextColor
                TextButton.TextSize = 20.000
                TextButton.Text = title
                UICorner_5.CornerRadius = UDim.new(0, 5)
                UICorner_5.Parent = TextButton

                touch_app.Name = "touch_app"
                touch_app.Parent = Button
                touch_app.BackgroundTransparency = 1.000
                touch_app.LayoutOrder = 9
                touch_app.Position = UDim2.new(0, 197, 0, 5)
                touch_app.Size = UDim2.new(0, 26, 0, 22)
                touch_app.ZIndex = 11

                touch_app.Image = "rbxassetid://3926305904"
                touch_app.ImageRectOffset = Vector2.new(84, 204)
                touch_app.ImageRectSize = Vector2.new(36, 36)

                TextButton.MouseButton1Down:Connect(function()
                     RippleEffect(Button)               
                    pcall(callback)
                end)
            end
            function Content:CreateToggle(title,default,callback)
                local Toggled = false
                local ToggleFunc = {}
                local Toggle = Instance.new("Frame")
                local Title = Instance.new("TextLabel")
                local ToggleBack = Instance.new("TextButton")
                local UICorner = Instance.new("UICorner")
                local ImageLabel = Instance.new("ImageLabel")
                local UICorner_2 = Instance.new("UICorner")

                Toggle.Name = title
                Toggle.Parent = SectionHold
                Toggle.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                Toggle.BackgroundTransparency = 1.000
                Toggle.BorderSizePixel = 0
                Toggle.Position = UDim2.new(0, 0, 0, 187)
                Toggle.Size = UDim2.new(0, 231, 0, 30)
                Toggle.ZIndex = 7

                Title.Name = "Title"
                Title.Parent = Toggle
                Title.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                Title.BackgroundTransparency = 1.000
                Title.Position = UDim2.new(0, 43, 0, 6)
                Title.Size = UDim2.new(0, 168, 0, 22)
                Title.ZIndex = 8
                Title.Font = Enum.Font.SourceSansBold
                Title.Text = title
                Title.TextColor3 = theme.TextColor
                Title.TextSize = 20.000
                Title.TextXAlignment = Enum.TextXAlignment.Left

                ToggleBack.Name = "ToggleBack"
                ToggleBack.Parent = Toggle
                ToggleBack.BackgroundColor3 = theme.Header
                ToggleBack.Position = UDim2.new(0.0173160173, 0, 0.0666666701, 0)
                ToggleBack.Size = UDim2.new(0, 26, 0, 26)
                ToggleBack.ZIndex = 11
                ToggleBack.ClipsDescendants = true
                ToggleBack.Font = Enum.Font.SourceSans
                ToggleBack.Text = ""
                ToggleBack.TextColor3 = Color3.fromRGB(0, 0, 0)
                ToggleBack.TextSize = 14.000

                UICorner.CornerRadius = UDim.new(0, 5)
                UICorner.Parent = ToggleBack
                function ToggleFunc:Update(state)
                    if state then
                        Toggled = state
                        TweenService:Create(
                            ImageLabel,
                            TweenInfo.new(.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out),
                            {BackgroundColor3 = Toggled and theme.SchemeColor or theme.Header}
                        ):Play()
                        pcall(callback,Toggled)
                    else
                        Toggled = state
                        TweenService:Create(
                            ImageLabel,
                            TweenInfo.new(.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out),
                            {BackgroundColor3 = Toggled and theme.SchemeColor or theme.Header}
                        ):Play()
                        pcall(callback,Toggled)
                    end
                end
                
                ToggleBack.MouseButton1Down:Connect(function()
                    Toggled = not Toggled
                    TweenService:Create(
                        ImageLabel,
                        TweenInfo.new(.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out),
                        {BackgroundColor3 = Toggled and theme.SchemeColor or theme.Header}
                    ):Play()
                    RippleEffect(ToggleBack)               

                    pcall(callback,Toggled)
                end)
                
                ImageLabel.Parent = ToggleBack
                ImageLabel.BackgroundColor3 = theme.Header
                ImageLabel.Position = UDim2.new(0, 1, 0, 1)
                ImageLabel.Size = UDim2.new(0, 24, 0, 24)
                ImageLabel.ZIndex = 11
                ImageLabel.Image = "rbxassetid://3926305904"
                ImageLabel.ImageColor3 = Color3.fromRGB(41, 41, 41)
                ImageLabel.ImageRectOffset = Vector2.new(312, 4)
                ImageLabel.ImageRectSize = Vector2.new(24, 24)

                UICorner_2.CornerRadius = UDim.new(0, 5)
                UICorner_2.Parent = ImageLabel

                if default then
                    Toggled = default
                    TweenService:Create(
                        ImageLabel,
                        TweenInfo.new(.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out),
                        {BackgroundColor3 = Toggled and theme.SchemeColor or theme.Header}
                    ):Play()
                    pcall(callback,Toggled)
                end
                return ToggleFunc
            end
            function Content:CreateKeybind(title,ori,callback)
                local Keybind = Instance.new("Frame")
                local Title_4 = Instance.new("TextLabel")
                local TextButton2323 = Instance.new("TextButton")
                local UICorner_5 = Instance.new("UICorner")
                Keybind.Name = title
                Keybind.Parent = SectionHold
                Keybind.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                Keybind.BackgroundTransparency = 1.000
                Keybind.BorderSizePixel = 0
                Keybind.Position = UDim2.new(0, 0, 0, 223)
                Keybind.Size = UDim2.new(0, 231, 0, 30)
                Keybind.ZIndex = 7

                Title_4.Name = "Title"
                Title_4.Parent = Keybind
                Title_4.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                Title_4.BackgroundTransparency = 1.000
                Title_4.BorderSizePixel = 0
                Title_4.Position = UDim2.new(0, 10, 0, 4)
                Title_4.Size = UDim2.new(0, 98, 0, 22)
                Title_4.ZIndex = 8
                Title_4.Font = Enum.Font.SourceSansBold
                Title_4.Text = title
                Title_4.TextColor3 = theme.TextColor
                Title_4.TextSize = 18.000
                Title_4.TextXAlignment = Enum.TextXAlignment.Left

                TextButton2323.Parent = Keybind
                TextButton2323.BackgroundColor3 = theme.Header
                TextButton2323.Position = UDim2.new(0.744588733, 0, 0.13333334, 0)
                TextButton2323.Size = UDim2.new(0, 65, 0, 24)
                TextButton2323.ZIndex = 11
                TextButton2323.Font = Enum.Font.SourceSansBold
                TextButton2323.TextColor3 = theme.TextColor
                TextButton2323.TextSize = 15.000
                TextButton2323.Text = ori.Name or ""
                UICorner_5.CornerRadius = UDim.new(0, 5)
                UICorner_5.Parent = TextButton2323
                TextButton2323.MouseButton1Click:Connect(function()
                    
                TextButton2323.Text = "..."
                    local inputwait = UserInputService.InputBegan:wait()
                    if inputwait.KeyCode.Name ~= "Unknown" then
                        TextButton2323.Text = inputwait.KeyCode.Name
                        Key = inputwait.KeyCode.Name
                    end
                end)
                    
                UserInputService.InputBegan:connect(
                function(current, pressed)
                    if not pressed then
                        if current.KeyCode.Name == Key then
                            pcall(callback)
                        end
                    end
                end)
            end
            function Content:CreateSlider(title,min,max,default,callback)
                local SliderFunc = {}
                local Slider = Instance.new("Frame")
                local Title_2 = Instance.new("TextLabel")
                local Frame = Instance.new("Frame")
                local UICorner_2 = Instance.new("UICorner")
                local Title_3 = Instance.new("TextLabel")
                local add = Instance.new("ImageButton")
                local remove = Instance.new("ImageButton")
                local SliderFrame = Instance.new("TextButton")
                local UICorner_3 = Instance.new("UICorner")
                local Sliderin = Instance.new("TextButton")
                local UICorner_4 = Instance.new("UICorner")
                Slider.Name = title
                Slider.Parent = SectionHold
                Slider.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                Slider.BackgroundTransparency = 1.000
                Slider.BorderSizePixel = 0
                Slider.Position = UDim2.new(0, 0, 0, 61)
                Slider.Size = UDim2.new(0, 231, 0, 39)
                Slider.ZIndex = 7
                
                Title_2.Name = "Title"
                Title_2.Parent = Slider
                Title_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                Title_2.BackgroundTransparency = 1.000
                Title_2.Position = UDim2.new(0.0519480482, 0, 0.128205135, 0)
                Title_2.Size = UDim2.new(0, 143, 0, 23)
                Title_2.ZIndex = 8
                Title_2.Font = Enum.Font.SourceSansBold
                Title_2.Text = title
                Title_2.TextColor3 = theme.TextColor
                Title_2.TextSize = 20.000
                Title_2.TextXAlignment = Enum.TextXAlignment.Left
                
                Frame.Parent = Slider
                Frame.BackgroundColor3 = theme.Header
                Frame.BorderColor3 = Color3.fromRGB(27, 42, 53)
                Frame.BorderSizePixel = 0
                Frame.Position = UDim2.new(0, 181, 0, 5)
                Frame.Size = UDim2.new(0, 30, 0, 19)
                Frame.ZIndex = 9
                
                UICorner_2.CornerRadius = UDim.new(0, 5)
                UICorner_2.Parent = Frame
                
                Title_3.Name = "Title"
                Title_3.Parent = Frame
                Title_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                Title_3.BackgroundTransparency = 1.000
                Title_3.BorderSizePixel = 0
                Title_3.Size = UDim2.new(0, 29, 0, 19)
                Title_3.ZIndex = 10
                Title_3.Font = Enum.Font.SourceSansBold
                Title_3.Text = "30"
                Title_3.TextColor3 = theme.TextColor
                Title_3.TextSize = 15.000
                
                add.Name = "add"
                add.Parent = Slider
                add.BackgroundTransparency = 1.000
                add.LayoutOrder = 3
                add.Position = UDim2.new(0, 210, 0, 4)
                add.Size = UDim2.new(0, 21, 0, 21)
                add.ZIndex = 9
                add.ClipsDescendants = true
                add.Image = "rbxassetid://3926307971"
                add.ImageRectOffset = Vector2.new(324, 364)
                add.ImageRectSize = Vector2.new(36, 36)
                
                remove.Name = "remove"
                remove.Parent = Slider
                remove.BackgroundTransparency = 1.000
                remove.LayoutOrder = 6
                remove.Position = UDim2.new(0, 156, 0, 4)
                remove.Size = UDim2.new(0, 21, 0, 21)
                remove.ZIndex = 9
                remove.ClipsDescendants = true
                remove.Image = "rbxassetid://3926307971"
                remove.ImageRectOffset = Vector2.new(884, 284)
                remove.ImageRectSize = Vector2.new(36, 36)
                
                SliderFrame.Name = "SliderFrame"
                SliderFrame.Parent = Slider
                SliderFrame.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                SliderFrame.Position = UDim2.new(0.012987013, 0, 0.717948735, 0)
                SliderFrame.Size = UDim2.new(0, 225, 0, 6)
                SliderFrame.ZIndex = 11
                SliderFrame.Font = Enum.Font.SourceSans
                SliderFrame.Text = ""
                SliderFrame.TextColor3 = Color3.fromRGB(0, 0, 0)
                SliderFrame.TextSize = 14.000
                
                UICorner_3.CornerRadius = UDim.new(0, 5)
                UICorner_3.Parent = SliderFrame
                
                Sliderin.Name = "Sliderin"
                Sliderin.Parent = SliderFrame
                Sliderin.BackgroundColor3 = theme.SchemeColor
                Sliderin.Size = UDim2.new(0, 125, 0, 6)
                Sliderin.ZIndex = 11
                Sliderin.Font = Enum.Font.SourceSans
                Sliderin.Text = ""
                Sliderin.TextColor3 = Color3.fromRGB(0, 0, 0)
                Sliderin.TextSize = 14.000
                
                UICorner_4.CornerRadius = UDim.new(0, 5)
                UICorner_4.Parent = Sliderin

                local mouse = game:GetService("Players").LocalPlayer:GetMouse();  

                local Value = default
                SliderFrame.MouseButton1Down:Connect(function()
                    if not focusing then
                        Value = math.floor((((tonumber(max) - tonumber(min)) / 225) * Sliderin.AbsoluteSize.X) + tonumber(min)) or 0
                        pcall(function()
                            callback(Value)
                        end)
                        Sliderin:TweenSize(UDim2.new(0, math.clamp(mouse.X - Sliderin.AbsolutePosition.X, 0, 225), 0, 6), "InOut", "Linear", 0.01, true)
                        moveconnection = mouse.Move:Connect(function()
                            Value = math.floor((((tonumber(max) - tonumber(min)) / 225) * Sliderin.AbsoluteSize.X) + tonumber(min))
                            Title_3.Text = Value
                            pcall(function()
                                callback(Value)
                            end)
                            Sliderin:TweenSize(UDim2.new(0, math.clamp(mouse.X - Sliderin.AbsolutePosition.X, 0, 225), 0, 6), "InOut", "Linear", 0.01, true)
                        end)
                        releaseconnection = UserInputService.InputEnded:Connect(function(Mouse)
                            if Mouse.UserInputType == Enum.UserInputType.MouseButton1 then
                                Value = math.floor((((tonumber(max) - tonumber(min)) / 225) * Sliderin.AbsoluteSize.X) + tonumber(min))
                                Title_3.Text = Value
    
                                pcall(function()
                                    callback(Value)
                                end)
    
                                Sliderin:TweenSize(UDim2.new(0, math.clamp(mouse.X - Sliderin.AbsolutePosition.X, 0, 225), 0, 6), "InOut", "Linear", 0.01, true)
                                moveconnection:Disconnect()
                                releaseconnection:Disconnect()
                            end
                        end)
                    end
                end)
                Sliderin.MouseButton1Down:Connect(function()
                    if not focusing then
                        Value = math.floor((((tonumber(max) - tonumber(min)) / 225) * Sliderin.AbsoluteSize.X) + tonumber(min)) or 0
                        pcall(function()
                            callback(Value)
                        end)
                        Sliderin:TweenSize(UDim2.new(0, math.clamp(mouse.X - Sliderin.AbsolutePosition.X, 0, 225), 0, 6), "InOut", "Linear", 0.01, true)
                        moveconnection = mouse.Move:Connect(function()
                            Value = math.floor((((tonumber(max) - tonumber(min)) / 225) * Sliderin.AbsoluteSize.X) + tonumber(min))
                            Title_3.Text = Value
                            pcall(function()
                                callback(Value)
                            end)
                            Sliderin:TweenSize(UDim2.new(0, math.clamp(mouse.X - Sliderin.AbsolutePosition.X, 0, 225), 0, 6), "InOut", "Linear", 0.01, true)
                        end)
                        releaseconnection = UserInputService.InputEnded:Connect(function(Mouse)
                            if Mouse.UserInputType == Enum.UserInputType.MouseButton1 then
                                Value = math.floor((((tonumber(max) - tonumber(min)) / 225) * Sliderin.AbsoluteSize.X) + tonumber(min))
                                Title_3.Text = Value
    
                                pcall(function()
                                    callback(Value)
                                end)
    
                                Sliderin:TweenSize(UDim2.new(0, math.clamp(mouse.X - Sliderin.AbsolutePosition.X, 0, 225), 0, 6), "InOut", "Linear", 0.01, true)
                                moveconnection:Disconnect()
                                releaseconnection:Disconnect()
                            end
                        end)
                    end
                end)
                add.MouseButton1Click:Connect(function()
                    Value = math.clamp(Value + 1, 1, max)
                    Sliderin.Size = UDim2.new(Value / max, 0, 0, 6)
                    Title_3.Text = Value
                    pcall(function()
                        callback(Value)
                    end)
                    RippleEffect(add)               

                end)

                remove.MouseButton1Click:Connect(function()
                    Value = math.clamp(Value - 1, min, max)
                    Sliderin.Size = UDim2.new(Value / max, 0, 0, 6)
                    Title_3.Text = Value
                    pcall(function()
                        callback(Value)
                    end)
                    RippleEffect(remove)               

                end)

                if default then
                    Sliderin.Size = UDim2.new((default or 0) / max, 0, 0, 6)
                    Title_3.Text = default
                    pcall(function()
                        callback(default)
                    end)
                end
                function SliderFunc:Update(value)
                    Sliderin.Size = UDim2.new((value or 0) / max, 0, 0, 6)
                    Title_3.Text = value
                    pcall(function()
                        callback(value)
                    end)
                end
                return SliderFunc
            end
            function Content:CreateTextBox(title,disapper,callback)
                local TextBox = Instance.new("Frame")
                local Title = Instance.new("TextLabel")
                local TextBox_2 = Instance.new("TextBox")
                local UICorner = Instance.new("UICorner")
                
                TextBox.Name = title
                TextBox.Parent = SectionHold
                TextBox.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                TextBox.BackgroundTransparency = 1.000
                TextBox.BorderSizePixel = 0
                TextBox.Position = UDim2.new(0, 0, 0, 187)
                TextBox.Size = UDim2.new(0, 231, 0, 30)
                TextBox.ZIndex = 7
                
                Title.Name = "Title"
                Title.Parent = TextBox
                Title.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                Title.BackgroundTransparency = 1.000
                Title.BorderSizePixel = 0
                Title.Position = UDim2.new(0, 20, 0, 5)
                Title.Size = UDim2.new(0, 98, 0, 22)
                Title.ZIndex = 8
                Title.Font = Enum.Font.SourceSansBold
                Title.Text = title
                Title.TextColor3 = theme.TextColor
                Title.TextSize = 20.000
                Title.TextXAlignment = Enum.TextXAlignment.Left
                
                TextBox_2.Parent = TextBox
                TextBox_2.BackgroundColor3 = theme.Header
                TextBox_2.Position = UDim2.new(0.597402573, 0, 0.166666672, 0)
                TextBox_2.Size = UDim2.new(0, 83, 0, 22)
                TextBox_2.ZIndex = 11
                TextBox_2.Font = Enum.Font.SourceSans
                TextBox_2.Text = ""
                TextBox_2.TextColor3 = theme.TextColor
                TextBox_2.TextSize = 14.000
                
                UICorner.CornerRadius = UDim.new(0, 5)
                UICorner.Parent = TextBox_2 
                TextBox_2.FocusLost:Connect(
                    function(ep)
                        if ep then
                            if #TextBox_2.Text > 0 then
                                pcall(callback, TextBox_2.Text)
                                if disapper then
                                    TextBox_2.Text = ""
                                end
                            end
                        end
                    end
                )
            end
            function Content:CreateDropdown(title,list,callback)
                local DropFunc = {}
                local Droptog = false
                local Dropdown = Instance.new("Frame")
                local Title_5 = Instance.new("TextLabel")
                local Frame_2 = Instance.new("Frame")
                local UICorner_6 = Instance.new("UICorner")
                local TextLabel = Instance.new("TextLabel")
                local expand_more = Instance.new("ImageButton")
                local DropHold = Instance.new("Frame")
                local Droplis = Instance.new("ScrollingFrame")
                local UIListLayout23423423423 = Instance.new("UIListLayout")
                local UIPadding = Instance.new("UIPadding")
                local UICorner_8 = Instance.new("UICorner")
                            
                Dropdown.Name = title
                Dropdown.Parent = SectionHold
                Dropdown.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                Dropdown.BackgroundTransparency = 1.000
                Dropdown.BorderSizePixel = 0
                Dropdown.Position = UDim2.new(0, 0, 0, 187)
                Dropdown.Size = UDim2.new(0, 231, 0, 30)
                Dropdown.ZIndex = 7

                Title_5.Name = "Title"
                Title_5.Parent = Dropdown
                Title_5.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                Title_5.BackgroundTransparency = 1.000
                Title_5.BorderSizePixel = 0
                Title_5.Position = UDim2.new(0, 20, 0, 5)
                Title_5.Size = UDim2.new(0, 98, 0, 22)
                Title_5.ZIndex = 10
                Title_5.Font = Enum.Font.SourceSansBold
                Title_5.Text = title
                Title_5.TextColor3 = theme.TextColor
                Title_5.TextSize = 18.000
                Title_5.TextXAlignment = Enum.TextXAlignment.Left

                Frame_2.Parent = Dropdown
                Frame_2.BackgroundColor3 = theme.Header
                Frame_2.BorderColor3 = Color3.fromRGB(27, 42, 53)
                Frame_2.BorderSizePixel = 0
                Frame_2.Position = UDim2.new(0, 12, 0, 1)
                Frame_2.Size = UDim2.new(0, 212, 0, 31)
                Frame_2.ZIndex = 9

                UICorner_6.CornerRadius = UDim.new(0, 5)
                UICorner_6.Parent = Frame_2

                TextLabel.Parent = Frame_2
                TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                TextLabel.BackgroundTransparency = 1.000
                TextLabel.BorderColor3 = Color3.fromRGB(27, 42, 53)
                TextLabel.Size = UDim2.new(0, 59, 0, 24)
                TextLabel.ZIndex = 9
                TextLabel.Font = Enum.Font.SourceSansBold
                TextLabel.Text = ""
                TextLabel.TextColor3 = theme.TextColor
                TextLabel.TextSize = 20.000

                expand_more.Name = "expand_more"
                expand_more.Parent = Frame_2
                expand_more.BackgroundTransparency = 1.000
                expand_more.Position = UDim2.new(0.855562031, 0, 0.0551075041, 0)
                expand_more.Size = UDim2.new(0, 25, 0, 25)
                expand_more.ZIndex = 9
                expand_more.Image = "rbxassetid://3926305904"
                expand_more.ImageRectOffset = Vector2.new(564, 284)
                expand_more.ImageRectSize = Vector2.new(36, 36)
                expand_more.Rotation = 0
                
                DropHold.Name = "DropHold"
                DropHold.Parent = SectionHold
                DropHold.BackgroundColor3 = theme.Header
                DropHold.Position = UDim2.new(0, 0, 0.746887982, 0)
                DropHold.Size = UDim2.new(0, 500, 0, 0)
                DropHold.ZIndex = 10
                DropHold.Visible = false
                DropHold.BackgroundTransparency = 1

                Droplis.Name = "Droplis"
                Droplis.Parent = DropHold
                Droplis.Active = true
                Droplis.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
                Droplis.BackgroundTransparency = 1.000
                Droplis.Size = UDim2.new(0, 231, 0, 112)
                Droplis.ZIndex = 11
                Droplis.ScrollBarThickness = 0
                Droplis.Visible = false
                Droplis.Position = UDim2.new(0, 5, 0, 0)

                UIListLayout23423423423.Parent = Droplis
                UIListLayout23423423423.SortOrder = Enum.SortOrder.LayoutOrder

                UIPadding.Parent = Droplis
                UIPadding.PaddingTop = UDim.new(0, 3)
                
                expand_more.MouseButton1Click:Connect(function()
                    Droptog = not Droptog
                    DropHold.Visible = Droptog
                    Droplis.Visible = Droptog
                    if expand_more.Rotation == 90 then
                        TweenService:Create(
                            expand_more,
                            TweenInfo.new(.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out),
                            {Rotation = 0}
                        ):Play()
                    else
                        TweenService:Create(
                            expand_more,
                            TweenInfo.new(.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out),
                            {Rotation = 90}
                        ):Play()
                    end
                    TweenService:Create(
                        DropHold,
                        TweenInfo.new(.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out),
                        {Size = Droptog and UDim2.new(0, 500, 0, 80) or UDim2.new(0, 500, 0, 0)}
                    ):Play()
                end)
    
                UICorner_8.Parent = DropHold

                for i,v in next, list do

                    local DrioBy = Instance.new("TextButton")
                    local UICorner_7 = Instance.new("UICorner")
                    DrioBy.Name = "DrioBy"
                    DrioBy.Parent = Droplis
                    DrioBy.BackgroundColor3 = Color3.fromRGB(71, 71, 71)
                    DrioBy.Size = UDim2.new(0, 224, 0, 26)
                    DrioBy.ZIndex = 12
                    DrioBy.Text = v 
                    DrioBy.Font = Enum.Font.SourceSansBold
                    DrioBy.TextColor3 = theme.TextColor
                    DrioBy.TextSize = 16.000
    
                    UICorner_7.CornerRadius = UDim.new(0, 3)
                    UICorner_7.Parent = DrioBy
    
    
                    DrioBy.MouseButton1Click:Connect(function()
                        pcall(callback, v)
                        Title_5.Text = title .. " : ".. v
                        Droptog = not Droptog
                        DropHold.Visible = Droptog
                        Droplis.Visible = Droptog
                        if expand_more.Rotation == 90 then
                            TweenService:Create(
                                expand_more,
                                TweenInfo.new(.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out),
                                {Rotation = 0}
                            ):Play()
                        end 
                        TweenService:Create(
                            DropHold,
                            TweenInfo.new(.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out),
                            {Size = Droptog and UDim2.new(0, 500, 0, 80) or UDim2.new(0, 500, 0, 0)}
                        ):Play()
                    end)
                end

                function DropFunc:Clear()
                    for i, v in next, Droplis:GetChildren() do
                        if v.Name == "DrioBy" then
                            v:Destroy()
                        end
                    end
                    if Droptog == true then
                        Title_5.Text = Title
                    end
                end

                function DropFunc:Add(addtext)
                    local DrioBy = Instance.new("TextButton")
                    local UICorner_7 = Instance.new("UICorner")
                    DrioBy.Name = "DrioBy"
                    DrioBy.Parent = Droplis
                    DrioBy.BackgroundColor3 = Color3.fromRGB(71, 71, 71)
                    DrioBy.Size = UDim2.new(0, 224, 0, 26)
                    DrioBy.ZIndex = 12
                    DrioBy.Text = addtext 
                    DrioBy.Font = Enum.Font.SourceSansBold
                    DrioBy.TextColor3 = theme.TextColor
                    DrioBy.TextSize = 16.000
    
                    UICorner_7.CornerRadius = UDim.new(0, 3)
                    UICorner_7.Parent = DrioBy
    
    
                    DrioBy.MouseButton1Click:Connect(function()
                        pcall(callback, addtext)
                        Title_5.Text = title .. " : ".. addtext
                        Droptog = not Droptog
                        DropHold.Visible = Droptog
                        Droplis.Visible = Droptog
                        if expand_more.Rotation == 90 then
                            TweenService:Create(
                                expand_more,
                                TweenInfo.new(.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out),
                                {Rotation = 0}
                            ):Play()
                        end 
                        TweenService:Create(
                            DropHold,
                            TweenInfo.new(.3, Enum.EasingStyle.Quad, Enum.EasingDirection.Out),
                            {Size = Droptog and UDim2.new(0, 500, 0, 80) or UDim2.new(0, 500, 0, 0)}
                        ):Play()
                    end)
                end
            return DropFunc
            end
        return Content
    end
    return SectionContent
end
return tabs
end

local Window = library:CreateWindow("Winnable ❗ Hub",library.themes.original,Enum.KeyCode.RightControl)

local Tab1s = Window:CreateTab('Main')
local Tab1 = Tab1s:CreateSection('Main')
local Tab2 = Tab1s:CreateSection('Setting Farm')
local Lol = Window:CreateTab('Stats')
local Stats = Lol:CreateSection('Stats') 
local StatsPoint = Lol:CreateSection('StatsPoint')
local yyy = Window:CreateTab('Raid')
local Raid = yyy:CreateSection('Raid') 
local RaidA = yyy:CreateSection('Auto Raid')
local TapTp = Window:CreateTab('Teleport')
local page1 = TapTp:CreateSection('Teleport')
local page2 = TapTp:CreateSection('Setting Teleport')
local Tpaasd = Window:CreateTab('Shop')
local pagee = Tpaasd:CreateSection('Shop')
local pagee2 = Tpaasd:CreateSection('Fruits')
local M = Window:CreateTab('Misc')
local Misc = M:CreateSection('Misc')
local Misc2 = M:CreateSection(' ')



Old_World = false
New_World = false
SeaThird_World = false
local placeId = game.PlaceId
if placeId == 2753915549 then
Old_World = true  
elseif placeId == 4442272183 then
New_World = true
elseif placeId == 7449423635 then
SeaThird_World = true    
end

--------------------function farm 
function CheckLevel()
    local Lv = game:GetService("Players").LocalPlayer.Data.Level.Value
    if Old_World then
    if Lv == 1 or Lv <= 9 then -- Bandit
        Ms = "Bandit [Lv. 5]"
        NameQuest = "BanditQuest1" 
        QuestLv = 1
        Reward = "Reward:\n$350\n250 Exp."
        CFrameQ = CFrame.new(1060.9383544922, 16.455066680908, 1547.7841796875)
        CFrameMon = CFrame.new(1200.7680664063, 57.918930053711, 1531.2384033203)

    elseif Lv == 10 or Lv <= 14 then -- Monkey
        Ms = "Monkey [Lv. 14]"
        NameQuest = "JungleQuest"
        QuestLv = 1
        Reward = "Reward:\n$800\n1,800 Exp."
        CFrameQ = CFrame.new(-1601.6553955078, 36.85213470459, 153.38809204102)
        CFrameMon = CFrame.new(-1596.4732666016, 29.89605140686, 206.4541015625)

    elseif Lv == 15 or Lv <= 29 then -- Gorilla
        Ms = "Gorilla [Lv. 20]"
        NameQuest = "JungleQuest"
        QuestLv = 2
        Reward = "Reward:\n$1,200\n3,500 Exp."
        CFrameQ = CFrame.new(-1601.6553955078, 36.85213470459, 153.38809204102)
        CFrameMon = CFrame.new(-1226.5432128906, 6.1267290115356, -420.04034423828)

    
    elseif Lv == 30 or Lv <= 39 then -- Pirate
        Ms = "Pirate [Lv. 35]"
        NameQuest = "BuggyQuest1"
        QuestLv = 1
        Reward = "Reward:\n$3,000\n10,000 Exp."
        CFrameQ = CFrame.new(-1140.1761474609, 4.752049446106, 3827.4057617188)
        CFrameMon = CFrame.new(-1181.0485839844, 44.752029418945, 3834.82421875) --eiei

        
    elseif Lv == 40 or Lv <= 59 then -- Brute
        Ms = "Brute [Lv. 45]"
        NameQuest = "BuggyQuest1"
        QuestLv = 2
        Reward = "Reward:\n$3,500\n18,000 Exp."
        CFrameQ = CFrame.new(-1140.1761474609, 4.752049446106, 3827.4057617188)
        CFrameMon = CFrame.new(-1303.3735351563, 15.089874267578, 4293.6079101563)

    
    elseif Lv == 60 or Lv <= 74 then -- Desert Bandit
        Ms = "Desert Bandit [Lv. 60]"
        NameQuest = "DesertQuest"
        QuestLv = 1
        Reward = "Reward:\n$4,000\n35,000 Exp."
        CFrameQ = CFrame.new(896.51721191406, 6.4384617805481, 4390.1494140625)
        CFrameMon = CFrame.new(828.45727539063, 21.567289352417, 4495.2534179688)

    
    elseif Lv == 75 or Lv <= 89 then -- Desert Officer
        Ms = "Desert Officer [Lv. 70]"
        NameQuest = "DesertQuest"
        QuestLv = 2
        Reward = "Reward:\n$4,500\n50,000 Exp."
        CFrameQ = CFrame.new(896.51721191406, 6.4384617805481, 4390.1494140625)
        CFrameMon = CFrame.new(1547.1510009766, 14.452038764954, 4381.8002929688)

    
    elseif Lv == 90 or Lv <= 99 then -- Snow Bandit
        Ms = "Snow Bandit [Lv. 90]"
        NameQuest = "SnowQuest"
        QuestLv = 1
        Reward = "Reward:\n$5,000\n70,000 Exp."
        CFrameQ = CFrame.new(1386.8073730469, 87.272789001465, -1298.3576660156)
        CFrameMon = CFrame.new(1356.3028564453, 105.76865386963, -1328.2418212891)

    
    elseif Lv == 100 or Lv <= 119 then -- Snowman
        Ms = "Snowman [Lv. 100]"
        NameQuest = "SnowQuest"
        QuestLv = 2
        Reward = "Reward:\n$5,500\n120,000 Exp."
        CFrameQ = CFrame.new(1386.8073730469, 87.272789001465, -1298.3576660156)
        CFrameMon = CFrame.new(1218.7956542969, 138.01184082031, -1488.0262451172)

    
    elseif Lv == 120 or Lv <= 149 then -- Chief Petty Officer
        Ms = "Chief Petty Officer [Lv. 120]"
        NameQuest = "MarineQuest2"
        QuestLv = 1
        Reward = "Reward:\n$6,000\n180,000 Exp."
        CFrameQ = CFrame.new(-5035.49609375, 28.677835464478, 4324.1840820313)
        CFrameMon = CFrame.new(-4840.0737304688, 51.27169418335, 4527.6059570313)

    
    elseif Lv == 150 or Lv <= 174 then -- Sky Bandit
        Ms = "Sky Bandit [Lv. 150]"
        NameQuest = "SkyQuest"
        QuestLv = 1
        Reward = "Reward:\n$7,000\n250,000 Exp."
        CFrameQ = CFrame.new(-4842.1372070313, 717.69543457031, -2623.0483398438)
        CFrameMon = CFrame.new(-4955.6411132813, 365.46365356445, -2908.1865234375)

    
    elseif Lv == 175 or Lv <= 224 then -- Dark Master
        Ms = "Dark Master [Lv. 175]"
        NameQuest = "SkyQuest"
        QuestLv = 2
        Reward = "Reward:\n$7,500\n350,000 Exp."
        CFrameQ = CFrame.new(-4842.1372070313, 717.69543457031, -2623.0483398438)
        CFrameMon = CFrame.new(-5148.1650390625, 439.04571533203, -2332.9611816406)

    elseif Lv == 225 or Lv <= 274 then -- Toga Warrior
        Ms = "Toga Warrior [Lv. 225]"
        NameQuest = "ColosseumQuest"
        QuestLv = 1
        Reward = "Reward:\n$7,000\n700,000 Exp."
        CFrameQ = CFrame.new(-1577.7890625, 7.4151420593262, -2984.4838867188)
        CFrameMon = CFrame.new(-1872.5166015625, 49.080215454102, -2913.810546875)

    
    elseif Lv == 275 or Lv <= 299 then -- Gladiator
        Ms = "Gladiator [Lv. 275]"
        NameQuest = "ColosseumQuest"
        QuestLv = 2
        Reward = "Reward:\n$7,500\n1,000,000 Exp."
        CFrameQ = CFrame.new(-1577.7890625, 7.4151420593262, -2984.4838867188)
        CFrameMon = CFrame.new(-1521.3740234375, 81.203170776367, -3066.3139648438)

    
    elseif Lv == 300 or Lv <= 329 then -- Military Soldier
        Ms = "Military Soldier [Lv. 300]"
        NameQuest = "MagmaQuest"
        QuestLv = 1
        Reward = "Reward:\n$8,250\n1,300,000 Exp."
        CFrameQ = CFrame.new(-5316.1157226563, 12.262831687927, 8517.00390625)
        CFrameMon = CFrame.new(-5369.0004882813, 61.24352645874, 8556.4921875)

    
    elseif Lv == 330 or Lv <= 374 then -- Military Spy
        Ms = "Military Spy [Lv. 330]"
        NameQuest = "MagmaQuest"
        QuestLv = 2
        Reward = "Reward:\n$8,500\n1,850,000 Exp."
        CFrameQ = CFrame.new(-5316.1157226563, 12.262831687927, 8517.00390625)
        CFrameMon = CFrame.new(-5984.0532226563, 82.14656829834, 8753.326171875)

    elseif Lv == 375 or Lv <= 399 then -- Fishman Warrior
        Ms = "Fishman Warrior [Lv. 375]"
        NameQuest = "FishmanQuest"
        QuestLv = 1
        Reward = "Reward:\n$8,750\n2,500,000 Exp."
        CFrameQ = CFrame.new(61122.65234375, 18.497442245483, 1569.3997802734)
        CFrameMon = CFrame.new(60844.10546875, 98.462875366211, 1298.3985595703)

    
    elseif Lv == 400 or Lv <= 449 then -- Fishman Commando
        Ms = "Fishman Commando [Lv. 400]"
        NameQuest = "FishmanQuest"
        QuestLv = 2
        Reward = "Reward:\n$9,000\n3,000,000 Exp."
        CFrameQ = CFrame.new(61122.65234375, 18.497442245483, 1569.3997802734)
        CFrameMon = CFrame.new(61738.3984375, 64.207321166992, 1433.8375244141)

    
    elseif Lv == 450 or Lv <= 474 then -- God's Guard       
        Ms = "God's Guard [Lv. 450]"
        NameQuest = "SkyExp1Quest"
        QuestLv = 1
        Reward = "Reward:\n$8,750\n3,800,000 Exp."
        CFrameQ = CFrame.new(-4721.8603515625, 845.30297851563, -1953.8489990234)
        CFrameMon = CFrame.new(-4628.0498046875, 866.92877197266, -1931.2352294922)

    elseif Lv == 475 or Lv <= 524 then -- Shanda
        Ms = "Shanda [Lv. 475]"
        NameQuest = "SkyExp1Quest"
        QuestLv = 2
        Reward = "Reward:\n$9,000\n4,300,000 Exp."
        CFrameQ = CFrame.new(-7863.1596679688, 5545.5190429688, -378.42266845703)
        CFrameMon = CFrame.new(-7685.1474609375, 5601.0751953125, -441.38876342773)
    
    elseif Lv == 525 or Lv <= 549 then -- Royal Squad
        Ms = "Royal Squad [Lv. 525]"
        NameQuest = "SkyExp2Quest"
        QuestLv = 1
        Reward = "Reward:\n$9,500\n4,600,000 Exp."
        CFrameQ = CFrame.new(-7903.3828125, 5635.9897460938, -1410.923828125)
        CFrameMon = CFrame.new(-7654.2514648438, 5637.1079101563, -1407.7550048828)
    
    elseif Lv == 550 or Lv <= 624 then -- Royal Soldier
        Ms = "Royal Soldier [Lv. 550]"
        NameQuest = "SkyExp2Quest"
        QuestLv = 2
        Reward = "Reward:\n$9,750\n5,000,000 Exp." 
        CFrameQ = CFrame.new(-7903.3828125, 5635.9897460938, -1410.923828125)
        CFrameMon = CFrame.new(-7760.4106445313, 5679.9077148438, -1884.8112792969)
    elseif Lv == 625 or Lv <= 649 then
        Ms = "Galley Pirate [Lv. 625]"
        NameQuest = "FountainQuest"
        QuestLv = 1
        Reward = "Reward:\n$10,000\n5,800,000 Exp."
        CFrameQ = CFrame.new(5253.5747070313, 38.526943206787, 4049.3862304688)
        CFrameMon = CFrame.new(5557.1684570313, 152.32717895508, 3998.7758789063)
    
    elseif Lv >= 650 then -- Galley Captain
        Ms = "Galley Captain [Lv. 650]"
        NameQuest = "FountainQuest"
        QuestLv = 2
        Reward = "Reward:\n$10,000\n6,300,000 Exp."
        CFrameQ = CFrame.new(5253.5747070313, 38.526943206787, 4049.3862304688)
        CFrameMon = CFrame.new(5677.6772460938, 92.786109924316, 4966.6323242188)
    end
end
    if New_World then
    if Lv == 700 or Lv <= 724 then -- Raider
        Ms = "Raider [Lv. 700]"
        NameQuest = "Area1Quest"
        QuestLv = 1
        Reward = "Reward:\n$10,250\n6,750,000 Exp."
        CFrameQ = CFrame.new(-427.72567749023, 72.99634552002, 1835.9426269531)
        CFrameMon = CFrame.new(68.874565124512, 93.635643005371, 2429.6752929688)
    elseif Lv == 725 or Lv <= 774 then -- Mercenary
        Ms = "Mercenary [Lv. 725]"
        NameQuest = "Area1Quest"
        QuestLv = 2
        Reward = "Reward:\n$10,500\n7,000,000 Exp."
        CFrameQ = CFrame.new(-427.72567749023, 72.99634552002, 1835.9426269531)
        CFrameMon = CFrame.new(-864.85009765625, 122.47104644775, 1453.1505126953)
    elseif Lv == 775 or Lv <= 874 then -- Swan Pirate
        Ms = "Swan Pirate [Lv. 775]"
        NameQuest = "Area2Quest"
        QuestLv = 1
        Reward = "Reward:\n$10,750\n7,500,000 Exp."
        CFrameQ = CFrame.new(635.61151123047, 73.096351623535, 917.81298828125)
        CFrameMon = CFrame.new(1065.3669433594, 137.64012145996, 1324.3798828125)
    elseif Lv == 875 or Lv <= 899 then -- Marine Lieutenant
        Ms = "Marine Lieutenant [Lv. 875]"
        NameQuest = "MarineQuest3"
        QuestLv = 1
        Reward = "Reward:\n$11,250\n9,000,000 Exp."
        CFrameQ = CFrame.new(-2440.9934082031, 73.04190826416, -3217.7082519531)
        CFrameMon = CFrame.new(-2489.2622070313, 84.613594055176, -3151.8830566406)
    elseif Lv == 900 or Lv <= 949 then -- Marine Captain
        Ms = "Marine Captain [Lv. 900]"
        NameQuest = "MarineQuest3"
        QuestLv = 2
        Reward = "Reward:\n$11,500\n10,500,000 Exp."
        CFrameQ = CFrame.new(-2440.9934082031, 73.04190826416, -3217.7082519531)
        CFrameMon = CFrame.new(-2335.2026367188, 79.786659240723, -3245.8674316406)
    elseif Lv == 950 or Lv <= 974 then -- Zombie
        Ms = "Zombie [Lv. 950]"
        NameQuest = "ZombieQuest"
        QuestLv = 1
        Reward = "Reward:\n$11,750\n11,000,000 Exp."
        CFrameQ = CFrame.new(-5494.3413085938, 48.505931854248, -794.59094238281)
        CFrameMon = CFrame.new(-5536.4970703125, 101.08577728271, -835.59075927734)
    elseif Lv == 975 or Lv <= 999 then -- Vampire
        Ms = "Vampire [Lv. 975]"
        NameQuest = "ZombieQuest"
        QuestLv = 2
        Reward = "Reward:\n$12,000\n12,000,000 Exp."
        CFrameQ = CFrame.new(-5494.3413085938, 48.505931854248, -794.59094238281)
        CFrameMon = CFrame.new(-5806.1098632813, 16.722528457642, -1164.4384765625)
    elseif Lv == 1000 or Lv <= 1049 then -- Snow Trooper
        Ms = "Snow Trooper [Lv. 1000]"
        NameQuest = "SnowMountainQuest"
        QuestLv = 1
        Reward = "Reward:\n$12,250\n13,000,000 Exp."
        CFrameQ = CFrame.new(607.05963134766, 401.44781494141, -5370.5546875)
        CFrameMon = CFrame.new(535.21051025391, 432.74209594727, -5484.9165039063)
    elseif Lv == 1050 or Lv <= 1099 then -- Winter Warrior
        Ms = "Winter Warrior [Lv. 1050]"
        NameQuest = "SnowMountainQuest"
        QuestLv = 2
        Reward = "Reward:\n$12,500\n14,200,000 Exp."
        CFrameQ = CFrame.new(607.05963134766, 401.44781494141, -5370.5546875)
        CFrameMon = CFrame.new(1234.4449462891, 456.95419311523, -5174.130859375)
    elseif Lv == 1100 or Lv <= 1124 then -- Lab Subordinate
        Ms = "Lab Subordinate [Lv. 1100]"
        NameQuest = "IceSideQuest"
        QuestLv = 1
        Reward = "Reward:\n$12,250\n15,500,000 Exp."
        CFrameQ = CFrame.new(-6061.841796875, 15.926671981812, -4902.0385742188)
        CFrameMon = CFrame.new(-5720.5576171875, 63.309471130371, -4784.6103515625)
    elseif Lv == 1125 or Lv <= 1174 then -- Horned Warrior
        Ms = "Horned Warrior [Lv. 1125]"
        NameQuest = "IceSideQuest"
        QuestLv = 2
        Reward = "Reward:\n$12,500\n16,800,000 Exp."
        CFrameQ = CFrame.new(-6061.841796875, 15.926671981812, -4902.0385742188)
        CFrameMon = CFrame.new(-6292.751953125, 91.181983947754, -5502.6499023438)
    elseif Lv == 1175 or Lv <= 1199 then -- Magma Ninja
        Ms = "Magma Ninja [Lv. 1175]"
        NameQuest = "FireSideQuest"
        QuestLv = 1
        Reward = "Reward:\n$12,250\n18,000,000 Exp."
        CFrameQ = CFrame.new(-5429.0473632813, 15.977565765381, -5297.9614257813)
        CFrameMon = CFrame.new(-5461.8388671875, 130.36347961426, -5836.4702148438)
    elseif Lv == 1200 or Lv <= 1249 then -- Lava Pirate
        Ms = "Lava Pirate [Lv. 1200]"
        NameQuest = "FireSideQuest"
        QuestLv = 2
        Reward = "Reward:\n$12,500\n20,000,000 Exp."
        CFrameQ = CFrame.new(-5429.0473632813, 15.977565765381, -5297.9614257813)
        CFrameMon = CFrame.new(-5251.1889648438, 55.164535522461, -4774.4096679688)
    elseif Lv == 1250 or Lv <= 1274 then
        Ms = "Ship Deckhand [Lv. 1250]"
        NameQuest = "ShipQuest1"
        QuestLv = 1
        Reward = "Reward:\n$12,250\n23,000,000 Exp."
        CFrameQ = CFrame.new(1040.2927246094, 125.08293151855, 32911.0390625)
        CFrameMon = CFrame.new(921.12365722656, 125.9839553833, 33088.328125)
    elseif Lv == 1275 or Lv <= 1299 then
        Ms = "Ship Engineer [Lv. 1275]"
        NameQuest = "ShipQuest1"
        QuestLv = 2
        Reward = "Reward:\n$12,500\n24,500,000 Exp."
        CFrameQ = CFrame.new(1040.2927246094, 125.08293151855, 32911.0390625)
        CFrameMon = CFrame.new(916.82257080078, 43.569816589355, 32778.26953125)
    elseif Lv == 1300 or Lv <= 1324 then
        Ms = "Ship Steward [Lv. 1300]"
        NameQuest = "ShipQuest2"
        QuestLv = 1
        Reward = "Reward:\n$12,250\n26,500,000 Exp."
        CFrameQ = CFrame.new(971.42065429688, 125.08293151855, 33245.54296875)
        CFrameMon = CFrame.new(943.85504150391, 129.58183288574, 33444.3671875)
    elseif Lv == 1325 or Lv <= 1349 then
        Ms = "Ship Officer [Lv. 1325]"
        NameQuest = "ShipQuest2"
        QuestLv = 2
        Reward = "Reward:\n$12,500\n28,500,000 Exp."
        CFrameQ = CFrame.new(971.42065429688, 125.08293151855, 33245.54296875)
        CFrameMon = CFrame.new(955.38458251953, 181.08335876465, 33331.890625)
    elseif Lv == 1350 or Lv <= 1374 then -- Arctic Warrior
        Ms = "Arctic Warrior [Lv. 1350]"
        NameQuest = "FrostQuest"
        QuestLv = 1
        Reward = "Reward:\n$12,250\n30,000,000 Exp."
        CFrameQ = CFrame.new(5668.1372070313, 28.202531814575, -6484.6005859375)
        CFrameMon = CFrame.new(5935.4541015625, 77.26016998291, -6472.7568359375)
    elseif Lv == 1375 or Lv <= 1424 then -- Snow Lurker
        Ms = "Snow Lurker [Lv. 1375]"
        NameQuest = "FrostQuest"
        QuestLv = 2
        Reward = "Reward:\n$12,500\n32,000,000 Exp."
        CFrameQ = CFrame.new(5668.1372070313, 28.202531814575, -6484.6005859375)
        CFrameMon = CFrame.new(5628.482421875, 57.574996948242, -6618.3481445313)
    elseif Lv == 1425 or Lv <= 1449 then -- Sea Soldier
        Ms = "Sea Soldier [Lv. 1425]"
        NameQuest = "ForgottenQuest"
        QuestLv = 1
        Reward = "Reward:\n$12,250\n33,500,000 Exp."
        CFrameQ = CFrame.new(-3054.5827636719, 236.87213134766, -10147.790039063)
        CFrameMon = CFrame.new(-3185.0153808594, 58.789089202881, -9663.6064453125)
    elseif Lv >= 1450 then -- Water Fighter
        Ms = "Water Fighter [Lv. 1450]"
        NameQuest = "ForgottenQuest"
        QuestLv = 2
        Reward = "Reward:\n$12,500\n35,500,000 Exp."
        CFrameQ = CFrame.new(-3053.8479003906, 236.87213134766, -10144.774414063)
        CFrameMon = CFrame.new(-3262.9301757813, 298.69036865234, -10552.529296875)
    end
    end
    
    if SeaThird_World then
    if Lv == 1500 or Lv <= 1529 then -- Pirate Millionaire
        Ms = "Pirate Millionaire [Lv. 1500]"
        NameQuest = "PiratePortQuest"
        QuestLv = 1
        Reward = "Reward:\n$13,000\n35,000,000 Exp."
        CFrameQ = CFrame.new(-288.67205810547, 43.819011688232, 5578.2158203125) 
        CFrameMon = CFrame.new(-116.27030181885, 85.058494567871, 5675.0864257813)
    elseif Lv == 1530 or Lv <= 1574 then -- Pistol Billionaire
        Ms = "Pistol Billionaire [Lv. 1525]"
        NameQuest = "PiratePortQuest"
        QuestLv = 2
        Reward = "Reward:\n$15,000\n37,500,000 Exp."
        CFrameQ = CFrame.new(-288.67205810547, 43.819011688232, 5578.2158203125)
        CFrameMon = CFrame.new(-341.73947143555, 144.3151550293, 6042.8999023438)
    elseif Lv == 1575 or Lv <= 1599 then -- Dragon Crew Warrior
        Ms = "Dragon Crew Warrior [Lv. 1575]"
        NameQuest = "AmazonQuest"
        QuestLv = 1
        Reward = "Reward:\n$13,000\n40,000,000 Exp."
        CFrameQ = CFrame.new(5833.7348632813, 51.377155303955, -1103.7581787109)
        CFrameMon = CFrame.new(6321.751953125, 84.189949035645, -1253.9689941406)
    elseif Lv == 1600 or Lv <=  1625 then -- Dragon Crew Archer
        Ms = "Dragon Crew Archer [Lv. 1600]"
        NameQuest = "AmazonQuest"
        QuestLv = 2
        Reward = "Reward:\n$15,000\n42,500,000 Exp."
        CFrameQ = CFrame.new(5833.7348632813, 51.377155303955, -1103.7581787109)
        CFrameMon = CFrame.new(6637.1337890625, 441.76708984375, 480.45645141602)
    elseif Lv == 1624 or Lv <= 1649 then -- Female Islander
        Ms = "Female Islander [Lv. 1625]"
        NameQuest = "AmazonQuest2"
        QuestLv = 1
        Reward = "Reward:\n$13,000\n45,500,000 Exp."
        CFrameQ = CFrame.new(5446.7407226563, 601.62945556641, 750.45581054688)
        CFrameMon = CFrame.new(4587.3745117188, 857.02606201172, 716.54608154297)
    elseif Lv == 1650 or Lv <= 1699 then -- Giant Islander
        Ms = "Giant Islander [Lv. 1650]"
        NameQuest = "AmazonQuest2"
        QuestLv = 2
        Reward = "Reward:\n$15,000\n48,000,000 Exp."
        CFrameQ = CFrame.new(5446.7407226563, 601.62945556641, 750.45581054688)
        CFrameMon = CFrame.new(5201.60546875, 684.40661621094, -93.565208435059)
    elseif Lv == 1700 or Lv <= 1724 then -- Marine Commodore
        Ms = "Marine Commodore [Lv. 1700]"
        NameQuest = "MarineTreeIsland"
        QuestLv = 1
        Reward = "Reward:\n$13,000\n51,000,000 Exp."
        CFrameQ = CFrame.new(2179.1062011719, 28.731239318848, -6737.0224609375)
        CFrameMon = CFrame.new(2351.0073242188, 115.82643890381, -7648.5795898438)
    elseif Lv == 1725 or Lv <= 1774 then -- Marine Rear Admiral
        Ms = "Marine Rear Admiral [Lv. 1725]"
        NameQuest = "MarineTreeIsland"
        QuestLv = 2
        Reward = "Reward:\n$15,000\n53,500,000 Exp."
        CFrameQ = CFrame.new(2179.1062011719, 28.731239318848, -6737.0224609375)
        CFrameMon = CFrame.new(3316.2048339844, 391.21942138672, -7171.431640625)
    elseif Lv == 1775 or Lv <= 1799 then -- Fishman Raider
        Ms = "Fishman Raider [Lv. 1775]"
        NameQuest = "DeepForestIsland3"
        QuestLv = 1
        Reward = "Reward:\n$13,000\n56,000,000 Exp."
        CFrameQ = CFrame.new(-10584.555664063, 331.78845214844, -8758.30078125)
        CFrameMon = CFrame.new(-10345.95703125, 394.54016113281, -8378.0478515625)
    elseif Lv == 1800 or Lv <= 1899 then
        Ms = "Fishman Captain [Lv. 1800]"
        NameQuest = "DeepForestIsland3"
        QuestLv = 2
        Reward = "Reward:\n$15,000\n58,500,000 Exp."
        CFrameQ = CFrame.new(-10584.555664063, 331.78845214844, -8758.30078125)
        CFrameMon = CFrame.new(-10975.088867188, 460.49996948242, -8859.6708984375)
    elseif Lv == 1900 or Lv <= 1924 then
        Ms = "Jungle Pirate [Lv. 1900]"
        NameQuest = "DeepForestIsland2"
        QuestLv = 1
        Reward = "Reward:\n$13,000\n67,000,000 Exp."
        CFrameQ = CFrame.new(-12682.793945313, 390.88650512695, -9901.4091796875)
        CFrameMon = CFrame.new(-12089.387695313, 446.61639404297, -10559.4609375)
    elseif Lv == 1925 or Lv <= 1974 then
        Ms = "Musketeer Pirate [Lv. 1925]"
        NameQuest = "DeepForestIsland2"
        QuestLv = 2
        Reward = "Reward:\n$15,000\n70,000,000 Exp."
        CFrameQ = CFrame.new(-12682.793945313, 390.88650512695, -9901.4091796875)
        CFrameMon = CFrame.new(-13552.057617188, 416.32092285156, -9885.4326171875)
    elseif Lv == 1975 or Lv <= 1999 then
        Ms = "Reborn Skeleton [Lv. 1975]"
        NameQuest = "HauntedQuest1"
        QuestLv = 1
        Reward = "Reward:\n$13,000\n73,000,000 Exp."
        CFrameQ = CFrame.new(-9481.1240234375, 142.13066101074, 5566.0473632813)
        CFrameMon = CFrame.new(-8763.6962890625, 165.76463317871, 6158.6577148438)
    elseif Lv == 2000 or Lv <= 2024 then
        Ms = "Living Zombie [Lv. 2000]"
        NameQuest = "HauntedQuest1"
        QuestLv = 2
        Reward = "Reward:\n$13,250\n75,500,000 Exp."
        CFrameQ = CFrame.new(-9481.1240234375, 142.13066101074, 5566.0473632813)
        CFrameMon = CFrame.new(-10193.255859375, 139.65251159668, 5984.3876953125)
    elseif Lv == 2025 or Lv <= 2074 then
        Ms = "Demonic Soul [Lv. 2025]"
        NameQuest = "HauntedQuest2"
        QuestLv = 1
        Reward = "Reward:\n$13,500\n78,000,000 Exp."
        CFrameQ = CFrame.new(-9515.267578125, 172.13066101074, 6077.5986328125)
        CFrameMon = CFrame.new(-9498.8447265625, 172.13066101074, 6161.533203125)
    elseif Lv == 2075 or Lv <= 2099 then
        Ms = "Peanut Scout [Lv. 2075]"
        NameQuest = "NutsIslandQuest"
        QuestLv = 1
        Reward = "Reward:\n$14,000\n82,500,000 Exp."
        CFrameQ = CFrame.new(-2104.1787109375, 38.129970550537, -10194.196289062)
        CFrameMon = CFrame.new(-1914.2595214844, 171.53665161133, -10151.4921875)
    elseif Lv == 2100 or Lv <= 2124 then
        Ms = "Peanut President [Lv. 2100]"
        NameQuest = "NutsIslandQuest"
        QuestLv = 2
        Reward = "Reward:\n$14,100\n84,500,000 Exp."
        CFrameQ = CFrame.new(-2104.1787109375, 38.129970550537, -10194.196289062)
        CFrameMon = CFrame.new(-2209.6862792969, 140.69230651855, -10538.555664062)
    elseif Lv == 2125 or Lv <= 2149 then
        Ms = "Ice Cream Chef [Lv. 2125]"
        NameQuest = "IceCreamIslandQuest"
        QuestLv = 1
        Reward = "Reward:\n$14,200\n86,500,000 Exp."
        CFrameQ = CFrame.new(-820.61273193359, 65.845329284668, -10965.97265625)
        CFrameMon = CFrame.new(-742.4423828125, 126.89678192139, -11166.838867188)
    elseif Lv >= 2150 then
        Ms = "Ice Cream Commander [Lv. 2150]"
        NameQuest = "IceCreamIslandQuest"
        QuestLv = 2
        Reward = "Reward:\n$14,300\n89,000,000 Exp."
        CFrameQ = CFrame.new(-820.61273193359, 65.845329284668, -10965.97265625)
        CFrameMon = CFrame.new(-695.22576904297, 171.41047668457, -11208.48046875)
            end
        end
    end


if Old_World then
magbring = 240
elseif New_World then
magbring = 400
elseif  SeaThird_World then
magbring = 400
end


MagAnti = 350
if game:GetService("Players").LocalPlayer.Data.Level.Value == 275 or game:GetService("Players").LocalPlayer.Data.Level.Value <= 299 then
    MagAnti = 500
else
    MagAuti = 350
end
Tab1:CreateLabel("Autofarm")

Tab1:CreateLine()

Tab1:CreateToggle("Auto Farm Level",false,function(v)
    _G.AOTO = v
    if  _G.SelectToolWeapon == "" then
        if _G.AOTO == true then 
        library:Notification("Please select a weapon","Please select a weapon","Okay!")
        end
    else
    _G.AutoFarm = v
    _G.noclip = v
    _G.P = v
    end
end)
Tab1:CreateToggle("Auto Superhuman",false,function(v)
    Superhuman = v
end)

Wapon = {}
for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do  
    if v:IsA("Tool") then
        table.insert(Wapon ,v.Name)
    end
end
local SelectToolWeapona = Tab2:CreateDropdown("SelectWeapon",Wapon,function(a)
_G.SelectToolWeapon = a
end)

Tab2:CreateButton("RefeshWeapon",function()
SelectToolWeapona:Clear()
    Wapon = {}
    for i,v in pairs(game.Players.LocalPlayer.Backpack:GetChildren()) do  
        if v:IsA("Tool") then
            SelectToolWeapona:Add(v.Name)
        end
    end
    for i,v in pairs(game.Players.LocalPlayer.Character:GetChildren()) do  
        if v:IsA("Tool") then
            SelectToolWeapona:Add(v.Name)
        end
    end
end)

Tab2:CreateToggle("Anit Bug",true,function(v)
    _G.WTF1 = v
end)
spawn(function()
while _G.WTF1 do wait() 
    if _G.P == true then
        if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
        _G.WTF = false 
        elseif game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == true then 
        _G.WTF = true 
        end
    elseif _G.P == false then
        _G.WTF = false
    end
end
end)
Tab2:CreateToggle("BringMon",true,function(v)
    _G.Magnet = v
end)



Tab2:CreateToggle("Fast Attack",false,function(v)
    _G.FastAttk = v
    _G.FASTA = V
end)

_G.OPEN = false
spawn(function()
if _G.OPEN == true then
    _G.Number = 0
 elseif _G.OPEN == false then
     _G.Number = 1 
 end
end)

Tab2:CreateSlider("Magbring",100,1000,magbring,function(v)
    magbring = v
end)



Tab2:CreateSlider("MagAnti",100,1000,MagAnti,function(v)
    MagAnti = v
end)



    --Auto Stats

    
Stats:CreateToggle("Melee", false, function(vu)
Melee = vu
end)

Stats:CreateToggle("Defense", false, function(vu)
Defense = vu
end)

Stats:CreateToggle("Sword", false, function(vu)
Sword = vu
end)

Stats:CreateToggle("Gun", false, function(vu)
Gun = vu
end)

Stats:CreateToggle("Devil Fruit", false, function(vu)
DevilFruit = vu
end)

Point = 1
StatsPoint:CreateSlider("Point", 1,500,Point, function(v)
SelectPoint = v
end)

Raid:CreateToggle("Kill Aura",false,function(c)
_G.KillAura = c
end)

Raid:CreateToggle("Auto NextIsland",false,function(c)
_G.NextIsland = c
_G.noclip = c
end)

Raid:CreateToggle("Auto Awake",false,function(value)
_G.Awake = value
end)

Raid:CreateButton("Teleport To Lab",function()
if New_World then
    Tween(CFrame.new(-6438.73535, 250.645355, -4501.50684))
elseif SeaThird_World then
    Tween(CFrame.new(-5093.0385742188, 314.97863769531, -2924.8054199219))
end
end)

Raid:CreateButton("Teleport AwakeRoom", function()
if New_World then
    Tween(CFrame.new(266.227783, 1.39509034, 1857.00732))
elseif SeaThird_World then
    Tween(CFrame.new(-11559.21, 55.1389618, -7578.56396, 1, 0, 0, 0, 1, 0, 0, 0, 1))
end
end)

RaidA:CreateDropdown("Select Raid", {"Flame","Ice","Quake","Light","Dark","String","Rumble","Magma","Human: Buddha"}, function(v)
_G.SelectRaid = v
end)

RaidA:CreateToggle("Auto Raid",false,function(value)
_G.AutoRaid = value
end)

RaidA:CreateToggle("Auto Buy Chip",false,function(value)
_G.AutoBuychip = value
end)



if Old_World then
    page1:CreateButton("Start Island",function()
        Tween(CFrame.new(1071.2832, 16.3085976, 1426.86792))
    end)
    page1:CreateButton("Marine Start",function()
        Tween(CFrame.new(-2573.3374, 6.88881969, 2046.99817))
    end)
    page1:CreateButton("Middle Town",function()
        Tween(CFrame.new(-655.824158, 7.88708115, 1436.67908))
    end)
    page1:CreateButton("Jungle",function()
        Tween(CFrame.new(-1249.77222, 11.8870859, 341.356476))
    end)
    page1:CreateButton("Pirate Village",function()
        Tween(CFrame.new(-1122.34998, 4.78708982, 3855.91992))
    end)
    page1:CreateButton("Desert",function()
        Tween(CFrame.new(1094.14587, 6.47350502, 4192.88721))
    end)
    page1:CreateButton("Frozen Village",function()
        Tween(CFrame.new(1198.00928, 27.0074959, -1211.73376))
    end)
    page1:CreateButton("MarineFord",function()
        Tween(CFrame.new(-4505.375, 20.687294, 4260.55908))
    end)
    page1:CreateButton("Colosseum",function()
        Tween(CFrame.new(-1428.35474, 7.38933945, -3014.37305))
    end)
    page1:CreateButton("Sky island 1 ",function()
        Tween(CFrame.new(-4970.21875, 717.707275, -2622.35449))
    end)
    page1:CreateButton("Sky island 2 ",function()
        Tween(CFrame.new(-4813.0249, 903.708557, -1912.69055))
    end)
    page1:CreateButton("Sky island 3 ",function()
        Tween(CFrame.new(-7952.31006, 5545.52832, -320.704956))
    end)
    page1:CreateButton("Sky island 4 ",function()
        Tween(CFrame.new(-7793.43896, 5607.22168, -2016.58362))
    end)
    page1:CreateButton("Prison",function()
        Tween(CFrame.new(4854.16455, 5.68742752, 740.194641))
    end)
    page1:CreateButton("Magma Village",function()
        Tween(CFrame.new(-5231.75879, 8.61593437, 8467.87695))
    end)
    page1:CreateButton("UndeyWater City",function()
        Tween(CFrame.new(61163.8516, 11.7796879, 1819.78418))
    end)
    page1:CreateButton("Fountain City",function()
        Tween(CFrame.new(5132.7124, 4.53632832, 4037.8562))
    end)
    page1:CreateButton("House Cyborg's",function()
        Tween(CFrame.new(6262.72559, 71.3003616, 3998.23047))
    end)
    page1:CreateButton("Shank's Room",function()
        Tween(CFrame.new(-1442.16553, 29.8788261, -28.3547478))
    end)
    page1:CreateButton("Mob Island",function()
        Tween(CFrame.new(-2850.20068, 7.39224768, 5354.99268))
    end)
end   
 if New_World then
    page1:CreateButton("Dock",function()
        Tween(CFrame.new(82.9490662, 18.0710983, 2834.98779))
    end)
    page1:CreateButton("Kingdom of Rose",function()
        Tween(CFrame.new(-394.983521, 118.503128, 1245.8446))
    end)
    page1:CreateButton("Mansion",function()
        Tween(CFrame.new(-390.096313, 331.886475, 673.464966))
    end)
    page1:CreateButton("Flamingo Room",function()
        Tween(CFrame.new(2302.19019, 15.1778421, 663.811035))
    end)
    page1:CreateButton("Green Zone",function()
        Tween(CFrame.new(-2372.14697, 72.9919434, -3166.51416))
    end)
    page1:CreateButton("Cafe",function()
        Tween(CFrame.new(-385.250916, 73.0458984, 297.388397))
    end)
    page1:CreateButton("Factroy",function()
        Tween(CFrame.new(430.42569, 210.019623, -432.504791))
    end)
    page1:CreateButton("Colosseum",function()
        Tween(CFrame.new(-1836.58191, 44.5890656, 1360.30652))
    end)
    page1:CreateButton("Grave Island",function()
        Tween(CFrame.new(-5411.47607, 48.8234024, -721.272522))
    end)
    page1:CreateButton("Snow Mountain",function()
        Tween(CFrame.new(511.825226, 401.765198, -5380.396))
    end)
    page1:CreateButton("Cold Island",function()
        Tween(CFrame.new(-6026.96484, 14.7461271, -5071.96338))
    end)
    page1:CreateButton("Hot Island",function()
        Tween(CFrame.new(-5478.39209, 15.9775667, -5246.9126))
    end)
    page1:CreateButton("Cursed Ship",function()
        Tween(CFrame.new(902.059143, 124.752518, 33071.8125))
    end)
    page1:CreateButton("Ice Castle",function()
        Tween(CFrame.new(5400.40381, 28.21698, -6236.99219))
    end)
    page1:CreateButton("Forgotten Island",function()
        Tween(CFrame.new(-3043.31543, 238.881271, -10191.5791))
    end)
    page1:CreateButton("Usoapp Island",function()
        Tween(CFrame.new(4748.78857, 8.35370827, 2849.57959))
    end)
    page1:CreateButton("Minisky Island",function()
        Tween(CFrame.new(-260.358917, 49325.7031, -35259.3008))
    end)
end
if SeaThird_World then
    page1:CreateButton("Port Towen",function()
        Tween(CFrame.new(-610.309692, 57.8323097, 6436.33594))
    end)
    page1:CreateButton("Hydra Island",function()
        Tween(CFrame.new(5229.99561, 603.916565, 345.154022))
    end)
    page1:CreateButton("Great Tree",function()
        Tween(CFrame.new(2174.94873, 28.7312393, -6728.83154))
    end)
    page1:CreateButton("Castle on the Sea",function()
        Tween(CFrame.new(-5477.62842, 313.794739, -2808.4585))
    end)
    page1:CreateButton("Floating Turtle",function()
        Tween(CFrame.new(-10919.2998, 331.788452, -8637.57227))
    end)
    page1:CreateButton("Mansion",function()
        Tween(CFrame.new(-12553.8125, 332.403961, -7621.91748))
    end)
    page1:CreateButton("Secret Temple",function()
        Tween(CFrame.new(5217.35693, 6.56511116, 1100.88159))
    end)
    page1:CreateButton("Friendly Arena",function()
        Tween(CFrame.new(5220.28955, 72.8193436, -1450.86304))
    end)
    page1:CreateButton("Beautiful Pirate Domain",function()
        Tween(CFrame.new(5310.8095703125, 21.594484329224, 129.39053344727))
    end)
    page1:CreateButton("Teler Park",function()
        Tween(CFrame.new(-9512.3623046875, 142.13258361816, 5548.845703125))
    end)
end


page2:CreateButton("Old_World",function()
    local args = {
        [1] = "TravelMain"
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)
page2:CreateButton("New_World",function()
    local args = {
        [1] = "TravelDressrosa"
    }
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end)

page2:CreateButton("SeaThird_World",function()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("TravelZou")
end)

page2:CreateButton("Stop Tween",function()
    Tween(game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame)
end)

pagee:CreateLabel("RESETSTATS")

pagee:CreateButton("Reset Stats",function()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","Refund","2")
end)

pagee:CreateLabel("Buy Fighting Style")

pagee:CreateButton("Black Leg",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyBlackLeg")
    end)
    pagee:CreateButton("Electro",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectro")
    end)
    pagee:CreateButton("Fishman Karate",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyFishmanKarate")
    end)
    pagee:CreateButton("Dragon Claw",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","DragonClaw","1")
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","DragonClaw","2")
    end)
    pagee:CreateButton("Superhuman",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySuperhuman")
    end)
    pagee:CreateButton("Death Step",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyDeathStep")
    end)
    pagee:CreateButton("Sharkman Karate",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate")
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuySharkmanKarate")
    end)
    pagee:CreateButton("Electric Claw",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyElectricClaw")
    end)
    
    pagee:CreateLabel("Sworld")
    
    pagee:CreateButton("Bisento",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Bisento")
    end)
    
    pagee:CreateButton("Dual-Headed Blade",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Dual-Headed Blade")
    end)
    
    pagee:CreateButton("Soul Cane",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Soul Cane")
    end)
    
    pagee:CreateButton("Triple Katana",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Triple Katana")
    end)
    pagee:CreateButton("Pipe",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Pipe")
    end)
    pagee:CreateButton("Dual Katana",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Dual Katana")
    end)
    pagee:CreateButton("Iron Mace",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Iron Mace")
    end)
    
    pagee:CreateLabel("Buy Iime")
    
    pagee:CreateButton("Geppo",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyHaki","Geppo")
    end)
    pagee:CreateButton("Buso Haki",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyHaki","Buso")
    end)
    pagee:CreateButton("Ken Haki",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("KenTalk","Buy")
    end)
    pagee:CreateButton("Soru",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyHaki","Soru")
    end)
    pagee:CreateButton("Random Race",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","Reroll","2")
    end)
    pagee:CreateButton("Microchip [ Raw ]",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BlackbeardReward","Microchip","2")
    end)
    
    pagee:CreateLabel("Gun")
    
    pagee:CreateButton("Slingshot",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Slingshot")
    end)
    pagee:CreateButton("Musket",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Musket")
    end)
    pagee:CreateButton("Refined Slingshot",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Refined Slingshot")
    end)
    pagee:CreateButton("Cannon",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("BuyItem","Cannon")
    end)
    pagee:CreateButton("Bizarre Rifle",function()
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Ectoplasm","Buy",1)
    end)


    
    pagee2:CreateDropdown("DevilFruit Sinper",{
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
	"Shadow-Shadow",
	"Venom-Venom",
    "Control-Control",
    "Dragon-Dragon"
    },function(ply)
    SelectDevil = ply
end)
pagee2:CreateToggle("DevilFruit Sinper",false,function(vu)
    BuyFruitSinper = vu
    while BuyFruitSinper do wait()
        local args = {
            [1] = "GetFruits"
        }
        
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
        local args = {
            [1] = "PurchaseRawFruit",
            [2] = SelectDevil
        }
        
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end
end)

pagee2:CreateToggle("Auto Random Fruit",false,function(v)
	DevilAutoBuy = v
end)

spawn(function()
	while wait(1) do
		if DevilAutoBuy then wait()
			game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Cousin","Buy")
		end
	end
end)

pagee2:CreateToggle("Auto Drop Fruit", false, function(vu)
	Drop = vu
end)

spawn(function()
	while wait() do
		if Drop then
			pcall(function()
				for i,v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetChildren()) do
					if string.find(v.Name, "Fruit") then
						EquipWeapon(v.Name)
						SelectFruit = v.Name
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
						SelectFruit = v.Name
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

pagee2:CreateToggle("Bring Fruit",false,function(t)
	_G.BringFruit = t
end)

spawn(function()
	while wait() do
		if _G.BringFruit then
			pcall(function()
                if game:GetService("Players")["LocalPlayer"].PlayerGui.Main.Timer.Visible == false then
                    for i,v in pairs(game.Workspace:GetChildren()) do
                        if v:IsA("Tool") then
                            if (v.Handle.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude <= 20000 then
                                v.Handle.CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame
                            else 
                                TP2FF(v.Handle.CFrame)
                            end
                        end
                    end
                end
			end)
		end
	end
end)

pagee2:CreateToggle("Keep Fruit To Inventory",false,function(value)
	_G.Savefruit = value
end)

spawn(function()
	while wait() do
		if _G.Savefruit then
			wait(0.5)
			local a =     {
				"Bomb-Bomb",
				"Spike-Spike",
				"Chop-Chop",
				"Spring-Spring",
				"Kilo-Kilo",
				"Smoke-Smoke",
				"Spin-Spin",
				"Flame-Flame",
				"Brid:Falcon",
				"Ice-Ice",
				"Sand-Sand",
				"Dark-Dark",
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
				"Control-Control",
				"Dragon-Dragon"
			}
			pcall(function()  
				for i,v in pairs(a) do
					if _G.Savefruit then
						game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StoreFruit",v)
					end
				end
			end)
		end
 	end
end)


pagee2:CreateButton("Random Fruit", function()
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Cousin","Buy")
end)


Misc:CreateLabel("Esp")

Misc:CreateToggle("ESP Player",false,function(a)
	ESPPlayer = a
	while ESPPlayer do wait()
		UpdatePlayerChams()
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
							name.TextColor3 = Color3.new(255, 255 ,255)
						else
							name.TextColor3 = Color3.new(255, 255 ,255)
						end
					else
						v.Character.Head['NameEsp'..Number].TextLabel.Text = (v.Name ..'   \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Character.Head.Position).Magnitude/3) ..' M')
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

Misc:CreateToggle("ESP Chest",false,function(a)
	ChestESP = a
	while ChestESP do wait()
		UpdateChestChams() 
	end
end)

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
							if v.Name == "Chest1" then
								name.TextColor3 = Color3.fromRGB(255, 255, 255)
								name.Text = ("Chest 1" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
							end
							if v.Name == "Chest2" then
								name.TextColor3 = Color3.fromRGB(255, 255, 255)
								name.Text = ("Chest 2" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
							end
							if v.Name == "Chest3" then
								name.TextColor3 = Color3.fromRGB(255, 255 ,255)
								name.Text = ("Chest 3" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
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

Misc:CreateToggle("ESP Devil Fruit",false,function(a)
	DevilFruitESP = a
	while DevilFruitESP do wait()
		UpdateDevilChams() 
	end
end)

function UpdateDevilChams() 
	for i,v in pairs(game.Workspace:GetChildren()) do
		pcall(function()
			if DevilFruitESP then
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
						name.TextColor3 = Color3.fromRGB(255, 255 ,255)
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

Misc:CreateToggle("ESP Flower",false,function(a)
	FlowerESP = a
	while FlowerESP do wait()
		UpdateFlowerChams() 
	end
end)

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
						name.TextColor3 = Color3.fromRGB(255, 255 ,255)
						if v.Name == "Flower1" then 
							name.Text = ("Blue Flower" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
							name.TextColor3 = Color3.fromRGB(255, 255 ,255)
						end
						if v.Name == "Flower2" then
							name.Text = ("Red Flower" ..' \n'.. round((game:GetService('Players').LocalPlayer.Character.Head.Position - v.Position).Magnitude/3) ..' M')
							name.TextColor3 = Color3.fromRGB(255, 255 ,255)
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


Misc:CreateLabel("Animation")

Misc:CreateButton("Destroy animation", function()
	pcall(function()
		game:GetService("ReplicatedStorage").Assets.GUI:Destroy()
		game:GetService("ReplicatedStorage").Assets.SlashHit:Destroy()
		game:GetService("ReplicatedStorage").Effect.Container:Destroy()
	end)
end)

pcall(function()
	if _G.Deanimate then
	game:GetService("ReplicatedStorage").Assets.GUI:Destroy()
	game:GetService("ReplicatedStorage").Assets.SlashHit:Destroy()
	game:GetService("ReplicatedStorage").Effect.Container:Destroy()
	end
end)

Misc:CreateLabel("Open")

Misc:CreateButton("Open Awakening", function()
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AwakeningChanger","Check")
	game.Players.localPlayer.PlayerGui.Main.AwakeningToggler.Visible = true
end)

Misc:CreateButton("Open Inventory", function()
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("getInventoryWeapons")
	game.Players.localPlayer.PlayerGui.Main.Inventory.Visible = true
end)

Misc:CreateButton("Open Devil Shop", function()
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("GetFruits")
	game.Players.localPlayer.PlayerGui.Main.FruitShop.Visible = true
end)

Misc:CreateButton("Open Color Haki", function()
	game.Players.localPlayer.PlayerGui.Main.Colors.Visible = true
end)

Misc:CreateButton("Open Title Name", function()
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("getTitles")
	game.Players.localPlayer.PlayerGui.Main.Titles.Visible = true
end)

Misc:CreateLabel("Join Team")

Misc:CreateButton("Join Pirates", function()
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SetTeam","Pirates") 
end)

Misc:CreateButton("Join Marines Team", function()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("SetTeam","Marines") 
end)

Misc2:CreateLabel("Haki Stage")

Misc2:CreateButton("Stage 0", function()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ChangeBusoStage",0)
end)
Misc2:CreateButton("Stage 1", function()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ChangeBusoStage",1)
end)
Misc2:CreateButton("Stage 2", function()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ChangeBusoStage",2)
end)
Misc2:CreateButton("Stage 3", function()
    game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ChangeBusoStage",3)
end)
Misc2:CreateButton("Stage 4", function()
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ChangeBusoStage",4)
end)
Misc2:CreateButton("Stage 5", function()
	game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("ChangeBusoStage",5)
end)

Misc2:CreateLabel("Gui & FPS")

Misc2:CreateButton("FPS BOOST", function()
	if not game:IsLoaded() then repeat wait() until game:IsLoaded() end
if hookfunction and setreadonly then
    local mt = getrawmetatable(game)
    local old = mt.__newindex
    setreadonly(mt, false)
    local sda
    sda = hookfunction(old, function(t, k, v)
        if k == "Material" then
            if v ~= Enum.Material.Neon and v ~= Enum.Material.Plastic and v ~= Enum.Material.ForceField then v = Enum.Material.Plastic end
        elseif k == "TopSurface" then v = "Smooth"
        elseif k == "Reflectance" or k == "WaterWaveSize" or k == "WaterWaveSpeed" or k == "WaterReflectance" then v = 0
        elseif k == "WaterTransparency" then v = 1
        elseif k == "GlobalShadows" then v = false end
        return sda(t, k, v)
    end)
    setreadonly(mt, true)
end
local g = game
local w = g.Workspace
local l = g:GetService"Lighting"
local t = w:WaitForChild"Terrain"
t.WaterWaveSize = 0
t.WaterWaveSpeed = 0
t.WaterReflectance = 0
t.WaterTransparency = 1
l.GlobalShadows = false

function change(v)
    pcall(function()
        if v.Material ~= Enum.Material.Neon and v.Material ~= Enum.Material.Plastic and v.Material ~= Enum.Material.ForceField then
            pcall(function() v.Reflectance = 0 end)
            pcall(function() v.Material = Enum.Material.Plastic end)
            pcall(function() v.TopSurface = "Smooth" end)
        end
    end)
end

game.DescendantAdded:Connect(function(v)
    pcall(function()
        if v:IsA"Part" then change(v)
        elseif v:IsA"MeshPart" then change(v)
        elseif v:IsA"TrussPart" then change(v)
        elseif v:IsA"UnionOperation" then change(v)
        elseif v:IsA"CornerWedgePart" then change(v)
        elseif v:IsA"WedgePart" then change(v) end
    end)
end)
for i, v in pairs(game:GetDescendants()) do
    pcall(function()
        if v:IsA"Part" then change(v)
        elseif v:IsA"MeshPart" then change(v)
        elseif v:IsA"TrussPart" then change(v)
        elseif v:IsA"UnionOperation" then change(v)
        elseif v:IsA"CornerWedgePart" then change(v)
        elseif v:IsA"WedgePart" then change(v) end
    end)
end
end)

Misc2:CreateButton("Rejoin", function()
	game:GetService("TeleportService"):Teleport(game.PlaceId, game:GetService("Players").LocalPlayer)
end)

Misc2:CreateButton("Server Hop", function()
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
					wait(.1)
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

spawn(function()
while wait(.1) do
    if Superhuman then
        if game.Players.LocalPlayer.Backpack:FindFirstChild("Combat") or game.Players.LocalPlayer.Character:FindFirstChild("Combat") then
        local args = {
            [1] = "BuyBlackLeg"
        }
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
    end   
        if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") or game.Players.LocalPlayer.Character:FindFirstChild("Black Leg") or game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") or game.Players.LocalPlayer.Character:FindFirstChild("Electro") or game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") or game.Players.LocalPlayer.Character:FindFirstChild("Fishman Karate") or game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") or game.Players.LocalPlayer.Character:FindFirstChild("Dragon Claw") then
            if game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg") and game.Players.LocalPlayer.Backpack:FindFirstChild("Black Leg").Level.Value <= 299 then
                SelectToolWeapon = "Black Leg"
            end
            if game.Players.LocalPlayer.Backpack:FindFirstChild("Electro") and game.Players.LocalPlayer.Backpack:FindFirstChild("Electro").Level.Value <= 299 then
                SelectToolWeapon = "Electro"
            end
            if game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate") and game.Players.LocalPlayer.Backpack:FindFirstChild("Fishman Karate").Level.Value <= 299 then
                SelectToolWeapon = "Fishman Karate"
            end
            if game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw") and game.Players.LocalPlayer.Backpack:FindFirstChild("Dragon Claw").Level.Value <= 299 then
                SelectToolWeapon = "Dragon Claw"
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
                    game:GetService  ("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
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


spawn(function ()
while wait() do
    if _G.AutoBuychip then
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("RaidsNpc", "Select", _G.SelectRaid)
    end
end
end)


spawn(function()
while wait(.1) do
    if _G.AutoRaid then
        if not game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") then
            game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("RaidsNpc", "Select", _G.SelectRaid)
        end
        if not game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 1") and game.Players.LocalPlayer.Backpack:FindFirstChild("Special Microchip") or  game.Players.LocalPlayer.Character:FindFirstChild("Special Microchip")  then
            if New_World then
                fireclickdetector(game:GetService("Workspace").Map.CircleIsland.RaidSummon2.Button.Main.ClickDetector)
            elseif SeaThird_World then
                fireclickdetector(game:GetService("Workspace").Map["Boat Castle"].RaidSummon2.Button.Main.ClickDetector)
            end
        end
    end
end
end)




spawn(function()
while wait(.1) do
    if _G.Awake then
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Awakener","Check")
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("Awakener","Awaken")
    end
end
end)

spawn(function()
while wait(.1) do
    if _G.NextIsland or _G.AutoRaid then
        pcall(function()
            if game:GetService("Workspace").Map.RaidMap:FindFirstChild("RaidIsland5") or game:GetService("Workspace").Map.RaidMap:FindFirstChild("RaidIsland4") or game:GetService("Workspace").Map.RaidMap:FindFirstChild("RaidIsland3") or game:GetService("Workspace").Map.RaidMap:FindFirstChild("RaidIsland2") or game:GetService("Workspace").Map.RaidMap:FindFirstChild("RaidIsland1") then
                if game:GetService("Workspace").Map.RaidMap:FindFirstChild("RaidIsland5") then   
                    Tween(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 5").CFrame*CFrame.new(0,80,10))
                elseif game:GetService("Workspace").Map.RaidMap:FindFirstChild("RaidIsland4") then    
                    Tween(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 4").CFrame*CFrame.new(0,80,10))
                elseif game:GetService("Workspace").Map.RaidMap:FindFirstChild("RaidIsland3") then
                    Tween(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 3").CFrame*CFrame.new(0,80,10))                                 
                elseif game:GetService("Workspace").Map.RaidMap:FindFirstChild("RaidIsland2") then    
                    Tween(game:GetService("Workspace")["_WorldOrigin"].Locations:FindFirstChild("Island 2").CFrame*CFrame.new(0,80,10))
                elseif game:GetService("Workspace").Map.RaidMap:FindFirstChild("RaidIsland1") then
                    Tween(game:GetService("Workspace").Map.RaidMap:FindFirstChild("RaidIsland1"):FindFirstChildWhichIsA("Part").CFrame * CFrame.new(0,80,0))
                end
            else
                if New_World then
                    Tween(CFrame.new(-6438.73535, 250.645455, -4501.50584))
                elseif SeaThird_World then
                    Tween(CFrame.new(-5017.40869, 314.844055, -2823.0128))
                end
            end
        end)
    end
end
end)
spawn(function()
if _G.KillAura or _G.AutoRaid then
        for i,v in pairs(game.Workspace.Enemies:GetChildren()) do
            if _G.KillAura and (v.HumanoidRootPart.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= 500 then
                pcall(function()
                    v.HumanoidRootPart.Transparency = 1
                    v.HumanoidRootPart.Size = Vector3.new(50, 50, 50)
                    v.HumanoidRootPart.CanCollide = false
                    if v.Humanoid.Health > 0 then
                        v.Humanoid.Health = 0
                    elseif v.Humanoid.Health == 0 then
                        v.Humanoid.Health = v.Humanoid.MaxHealth
                    else
                        v.Humanoid.Health = 0
                    end
                end)
            end
        end
    end
end)



spawn(function()
while wait(.1) do
    if Melee then
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint", "Melee", SelectPoint)
    end
end
end)

spawn(function()

while wait(.1) do
    if Defense then
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint", "Defense", SelectPoint)
    end
end
end)

spawn(function()
while wait(.1) do
    if Sword then
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint", "Sword", SelectPoint)
    end
end
end)

spawn(function()
while wait(.1) do
    if Gun then
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint", "Gun", SelectPoint)
    end
end
end)

spawn(function()
while wait(.1) do
    if DevilFruit then
        game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("AddPoint", "Demon Fruit", SelectPoint)
    end
end
end)


local CMR = require(game.ReplicatedStorage.Util.CameraShaker)
local RigC = require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework) 
local VirtualUser = game:GetService('VirtualUser')

spawn(function()
game:GetService('RunService').Heartbeat:connect(function()
    if _G.FastAttk then
        pcall(function()
            CMR:Stop()
            game:GetService('RunService').Heartbeat:wait()
            game.Players.LocalPlayer.Character.Humanoid.Sit = false
            game.Players.LocalPlayer.Character.Busy.Value = false
            RigC.activeController.timeToNextAttack = tick() - 1942141
            RigC.activeController.hitboxMagnitude = 70
            RigC.activeController.attacking = false
            RigC.activeController.increment = 3
            RigC.activeController.humanoid.AutoRotate = true
            RigC.activeController.focusStart = 0 
            RigC.activeController.hitSound = Hit0
        end)
    end
end)
end)
spawn(function()
game:GetService('RunService').Heartbeat:connect(function()
    pcall(function()
    if _G.FastAttk then
    game:GetService('VirtualUser'):CaptureController()   
    game:GetService('VirtualUser'):Button1Down(Vector2.new(1280, 672))
  end
end)
end)
end)


function EquipWeapon(ToolSe)
if game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe) then
local tool = game.Players.LocalPlayer.Backpack:FindFirstChild(ToolSe)
wait(.4)
game.Players.LocalPlayer.Character.Humanoid:EquipTool(tool)
end
end

function Tween(P1)
pcall(function()
Distance = (P1.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
if Distance < 1000 then
Speed = 380
elseif Distance > 1000 then
Speed = 250
elseif Distance < 130 then
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = P1
end
game:GetService("TweenService"):Create(
game.Players.LocalPlayer.Character.HumanoidRootPart,
TweenInfo.new(Distance/Speed, Enum.EasingStyle.Linear),
{CFrame = P1}
):Play()
wait(Distance/Speed)
end)
end

function TweenMs(PQ)
pcall(function()
Distanc2e = (PQ.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).Magnitude
if Distanc2e < 250 then
Speed13 = 600
elseif Distanc2e < 500 then
Speed13 = 400
elseif Distanc2e < 1000 then
Speed13 = 350
elseif Distanc2e >= 1000 then
Speed13 = 200
end
game:GetService("TweenService"):Create(
game.Players.LocalPlayer.Character.HumanoidRootPart,
TweenInfo.new(Distanc2e/Speed13, Enum.EasingStyle.Linear),
{CFrame = PQ}
):Play()
end)
end



spawn(function()
game:GetService("RunService").Heartbeat:Connect(function()
wait(0.1)
if _G.noclip then
if not game:GetService("Workspace"):FindFirstChild("np") then
local np = Instance.new("Part")
np.Name = "np"
np.Parent = game.Workspace
np.Anchored = true
np.Transparency = _G.Number
np.Size = Vector3.new(30,-0.5,30)
np.Material = "Neon"
np.Color = Color3.fromRGB(0, 89, 255)
elseif game:GetService("Workspace"):FindFirstChild("np") then
game.Workspace["np"].CFrame = game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame * CFrame.new(0, -3.6, 0)
end
else
if game:GetService("Workspace"):FindFirstChild("np") then
game:GetService("Workspace"):FindFirstChild("np"):Destroy()
end
end
end)
end)

spawn(function()
game:GetService("RunService").Stepped:Connect(function()
if _G.noclip then
for _, v in pairs(game.Players.LocalPlayer.Character:GetDescendants()) do
if v:IsA("BasePart") then
    v.CanCollide = false
end
end
end
end)
end)

function K()
if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Container.QuestReward.Title.Text == Reward then
else
local args = {
[1] = "AbandonQuest"
}
game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end
end

spawn(function()
while wait() do
if _G.AutoFarm then
pcall(function()
repeat wait()
CheckLevel()
K()
if not game.Players.LocalPlayer.Character:FindFirstChild("HasBuso") then
local args = {
[1] = "Buso"
}
game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
end
if game:GetService("Players").LocalPlayer.PlayerGui.Main.Quest.Visible == false then
Tween(CFrameQ)
wait(.5)
game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer("StartQuest", NameQuest, QuestLv)
wait()
local args = {
    [1] = "SetSpawnPoint"
    }
game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))
else
for i,v in pairs(game:GetService("Workspace").Enemies:GetChildren()) do
        if v.Name == Ms then
                PosMonAutoFarm = v.HumanoidRootPart.CFrame
                v.HumanoidRootPart.Size = Vector3.new(60,60,60)
                v.HumanoidRootPart.CanCollide = false
                v.Humanoid:ChangeState(11)
                TweenMs(v.HumanoidRootPart.CFrame * CFrame.new(0,20,0))
                EquipWeapon(_G.SelectToolWeapon)
                game:GetService('VirtualUser'):CaptureController()
                game:GetService('VirtualUser'):Button1Down(Vector2.new(1280, 672))
            end
        end
    end
until _G.AutoFarm == false 
end)
end
end
end)

spawn(function()
while wait() do 
pcall(function()
game.Players.LocalPlayer.Character.Humanoid.Died:Connect(function()
_G.AutoFarm = false
wait(7)
Tween(game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame)
if _G.AOTO == true then
_G.AutoFarm = true
end
end)
end)
end
end)





spawn(function()
while wait() do
if _G.WTF then
if _G.AutoFarm then
pcall(function()
CheckLevel()
if (CFrameMon.Position - game.Players.LocalPlayer.Character.HumanoidRootPart.Position).magnitude > MagAnti then
    Tween(CFrameMon)
        end
end)
end
end
end
end)



while wait() do
if _G.Magnet then
if _G.AutoFarm then
CheckLevel()
pcall(function()
for k,x in pairs(game.Workspace.Enemies:GetChildren()) do
if x.Name == Ms and x:FindFirstChild("HumanoidRootPart") and x:FindFirstChild("Humanoid") and x.Humanoid.Health > 0 and (x.HumanoidRootPart.Position-game:GetService("Players").LocalPlayer.Character.HumanoidRootPart.Position).magnitude <= magbring then
    x.HumanoidRootPart.CFrame = PosMonAutoFarm
    sethiddenproperty(game.Players.LocalPlayer, "SimulationRadius", math.huge)
end 
end
end)
end
end
end

end--ห้ามลบ

loadsc()


