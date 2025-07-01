# Jade Dragon Snow Mountain
a MCP server for Jade Dragon Snow Mountain/玉龙雪山,enjoy live images, time-lapse videos, and current weather updates from multiple breathtaking viewpoints. Perfect for planning your trip or simply savoring nature in the moment . 实时领略丽江玉龙雪山的壮美风光 — 通过多个绝美视角呈现的直播画面、延时视频及最新天气信息。不论是规划行程，还是静赏自然美景，都再合适不过。

# Server Config
```
{
  "mcpServers": {
    "JadeDragonSnowMountain": {
      "command": "npx",
      "args": [
        "mcp-remote",
        "https://multiaidesk.com/api/destinations/mcp"
      ]
    }
  }
}
```

## for mcp client support http streamable , use this config:
```
"JadeDragonSnowMountain": {
  "type": "streamable-http",
  "url": "https://multiaidesk.com/api/destinations/mcp",
  "note": "For Streamable HTTP connections, add this URL directly in Client"
}
```

# Available Tools

* listDestinationsAndItsViewPoints
  Parameters:none
* getRealTimeImageOrTimelapseVideoUrlForDestination
  Parameters:
  destination_uid : unique id for interested destination
  stype: choose among image or video content, 'image' for real-time image, 'video' for time lapse video
  viewpoint_uid(optional): unique ID for specific viewpoint of selected destination
