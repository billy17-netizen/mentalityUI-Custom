# MentalityUI - Custom Edition

This is a custom fork of MentalityUI featuring additional functionality and QoL changes requested by the community.

## New Features & Changes

### 1. Advanced TabBox Customization
- Added support for icons inside \TabBox\ tabs.
- You can now use text-only, icon-only, or both text and icon on a single tab.
- Selected tab styling has been improved to sync perfectly with the active theme's \Accent\ color, providing a much cleaner visual indicator.

### 2. Live Window Stats (FPS & Ping)
- Added built-in toggles for real-time FPS and Ping indicators in the window header.
- Use \ShowFPS = true\ and \ShowPing = true\ when creating your \Library:Window()\.
- They feature a sleek, rounded pill design that integrates natively with the library's styling and theme colors.

### 3. OverlayList API (Spectator / Status Overlay)
- Added \Library:OverlayList(Data)\ to create generic floating overlay lists, similar to the existing KeybindList.
- Perfect for displaying Spectator Lists, Player Statuses, or Feature Information.
- Features complete background transparency syncing and automatic absolute size adjustments.
- **Example Usage:**

`lua
local SpectatorList = Library:OverlayList({
    Name = "Spectators",
    Icon = "eye" -- lucide icon name
})

-- Add items
local p1 = SpectatorList:Add("billy17-netizen", "[Admin]")

-- Update items dynamically
p1:Set("billy17-netizen", "[Owner]")

-- Remove an item
p1:Remove()

-- Clear the entire list
SpectatorList:Clear()
`

## Usage

Check out \example.lua\ for a complete walkthrough of all the features available in this UI library!
