---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: freedomrobotics.com
  spf: false
hosts:
- host: www.freedomrobotics.com
  https: false
kind: domain-security
layout: security
method: probed
name: Freedomrobotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freedom Robotics, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Freedom Robotics
provider_slug: freedomrobotics
slug: freedomrobotics-domain-security
source_filename: freedomrobotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.freedomrobotics.com\n  https: false\ndomains:\n- domain: freedomrobotics.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freedomrobotics/refs/heads/main/security/freedomrobotics-domain-security.yml
summary_line: DNSSEC
tags:
- Robotics
- Robot Fleet Management
- Fleet Operations
- Robotics Infrastructure
- Remote Teleoperation
- Robotics Observability
- ROS
- ROS 2
- Device Management
- Deployment Management
- Cobots
- AMR
- Drones
- Industrial Robots
- Embodied AI
---
