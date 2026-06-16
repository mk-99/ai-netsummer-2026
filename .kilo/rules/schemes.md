---
description: Network summer AI session - network diagrams building rules
agent: code
model: jetgpt/coding
---
# Network diagrams

## Format

Diagrams should be built in PlantUML format.

English text in plain ASCII encoding should be used for all descriptions.

## Styling

Network devices should be drawn as rectangles.

Host names should be placed inside these rectangles.

Use "spline" modifier for lines.

Do not use [hidden] or similar modifiers in square brackets.

## Layout

It is better to draw leaf switches below spine switches.

It is better to align devices in a row with similar functionality.

It is better to draw access switches below distribution switches.

It is better to draw distribution switches below core switches.

Internet access devices should be drawn at the top of the diagram.

Main devices and data centers should be grouped at the left side if possible, redundant devices and data centers should be grouped at the right side if possible.

## Connection labels

Labels of connection lines should be formatted as A -- B: label

Interfaces should be labeled as short as possible, e0/0/0 is better than Ethernet 0/0/0

IP addresses and masks should be formatted as 192.168.1.1/24

Routing protocols (OSPF, BGP, etc.) on overlay and underlay diagrams should be labeled on connections

## Color schemes

- Spines: pink
- Leaves: green
- Routers: blue
- Hosts: cyan
