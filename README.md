# Greymarch

Greymarch is a strategy-game prototype inspired by grand strategy titles like Age of History 2 and Hearts of Iron 4. The current build focuses on rendering a full-screen world map background, keeping the top and bottom edges visible while cropping the sides to fit the window.

## Current Features
- Full-screen map background rendered with MAUI.
- Map image included as a MAUI resource.
- Android and Windows targets enabled (iOS/Mac removed).

## Project Structure
- `Greymarch/` - MAUI app source.
- `Greymarch/MainPage.xaml` - Main UI that displays the map.
- `Greymarch/Resources/Images/mapchart_map.png` - Background map image.

## Build and Run
From the repository root:

```powershell
dotnet build
dotnet run --project Greymarch
```

## Notes
- The map is displayed using `AspectFill` to prioritize top and bottom visibility while cropping left/right edges.
