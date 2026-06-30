<style>#mermaid-1782804989482{font-family:sans-serif;font-size:16px;fill:#333;}@keyframes edge-animation-frame{from{stroke-dashoffset:0;}}@keyframes dash{to{stroke-dashoffset:0;}}#mermaid-1782804989482 .edge-animation-slow{stroke-dasharray:9,5!important;stroke-dashoffset:900;animation:dash 50s linear infinite;stroke-linecap:round;}#mermaid-1782804989482 .edge-animation-fast{stroke-dasharray:9,5!important;stroke-dashoffset:900;animation:dash 20s linear infinite;stroke-linecap:round;}#mermaid-1782804989482 .error-icon{fill:#552222;}#mermaid-1782804989482 .error-text{fill:#552222;stroke:#552222;}#mermaid-1782804989482 .edge-thickness-normal{stroke-width:1px;}#mermaid-1782804989482 .edge-thickness-thick{stroke-width:3.5px;}#mermaid-1782804989482 .edge-pattern-solid{stroke-dasharray:0;}#mermaid-1782804989482 .edge-thickness-invisible{stroke-width:0;fill:none;}#mermaid-1782804989482 .edge-pattern-dashed{stroke-dasharray:3;}#mermaid-1782804989482 .edge-pattern-dotted{stroke-dasharray:2;}#mermaid-1782804989482 .marker{fill:#333333;stroke:#333333;}#mermaid-1782804989482 .marker.cross{stroke:#333333;}#mermaid-1782804989482 svg{font-family:sans-serif;font-size:16px;}#mermaid-1782804989482 p{margin:0;}#mermaid-1782804989482 .node .neo-node{stroke:#9370DB;}#mermaid-1782804989482 [data-look="neo"].node rect,#mermaid-1782804989482 [data-look="neo"].cluster rect,#mermaid-1782804989482 [data-look="neo"].node polygon{stroke:#9370DB;filter:drop-shadow(1px 2px 2px rgba(185, 185, 185, 1));}#mermaid-1782804989482 [data-look="neo"].node path{stroke:#9370DB;stroke-width:1px;}#mermaid-1782804989482 [data-look="neo"].node .outer-path{filter:drop-shadow(1px 2px 2px rgba(185, 185, 185, 1));}#mermaid-1782804989482 [data-look="neo"].node .neo-line path{stroke:#9370DB;filter:none;}#mermaid-1782804989482 [data-look="neo"].node circle{stroke:#9370DB;filter:drop-shadow(1px 2px 2px rgba(185, 185, 185, 1));}#mermaid-1782804989482 [data-look="neo"].node circle .state-start{fill:#000000;}#mermaid-1782804989482 [data-look="neo"].icon-shape .icon{fill:#9370DB;filter:drop-shadow(1px 2px 2px rgba(185, 185, 185, 1));}#mermaid-1782804989482 [data-look="neo"].icon-shape .icon-neo path{stroke:#9370DB;filter:drop-shadow(1px 2px 2px rgba(185, 185, 185, 1));}#mermaid-1782804989482 :root{--mermaid-font-family:sans-serif;}#mermaid-1782804989482 :root{--mermaid-alt-font-family:sans-serif;}</style>

```mermaid
mindmap
root((Pac-Man))
 Theme
  เขาวงกต
  อาเขตยุค 80
 Mechanics
  เดินในเขาวงกต
  กิน Pellet
  Power Pellet
 Content
  ผีศัตรู 4 ตัว
  ผลไม้โบนัส
 Audience
  ผู้เล่น Casual
 Audio
  เสียงตัวละครเดิน
  เสียงตอนตาย
  เสียงตอนกินผลไม้โบนัส
 Art Style
  pixel art
```


```mermaid
quadrantChart
title Pac-Man — Feature Prioritization
x-axis Low Effort --> High Effort
y-axis Low Impact --> High Impact
quadrant-1 Quick Wins 
quadrant-2 Major
quadrant-3 Nice to Have
quadrant-4 Consider
Maze Movement: [0.3, 0.95]
Ghost AI: [0.7, 0.9]
Online Leaderboard: [0.7, 0.3]
Pellet Eating: [0.1, 0.9]
Score Count: [0.4, 0.9]
Cutscene: [0.4, 0.35]
Gameover: [0.3, 0.7]
```

Comment: MVP ซ้ายบน = Pellet Eating, MVP ขวาบน = Ghost AI, ตัด Cutscene กับ Online Leaderboard


```mermaid
gantt
title Pac-Man — Production Timeline (6 สัปดาห์)
dateFormat YYYY-MM-DD
section Pre-Production
Concept & GDD :done, c1, 2026-07-06, 5d
section Production
Maze Movement :active, p1, after c1, 5d
Ghost AI : p2, after p1, 7d
Pellet & Score : p3, after p2, 7d
section Post
QA & Bug Fix : q1, after p3, 5d
Beta :milestone, m2, after p3, 0d
Release Build :milestone, m1, after q1, 0d
```
