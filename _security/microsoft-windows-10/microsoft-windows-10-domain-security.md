---
api_specs:
- filename: microsoft-windows-10-winrt-openapi.yml
  format: yaml
  label: Windows Runtime (WinRT) API
  slug: windows-runtime-winrt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-winrt-openapi.yml
- filename: microsoft-windows-10-win32-openapi.yml
  format: yaml
  label: Win32 API
  slug: win32-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-win32-openapi.yml
- filename: microsoft-windows-10-notifications-openapi.yml
  format: yaml
  label: Windows Notifications API
  slug: windows-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-notifications-openapi.yml
- filename: microsoft-windows-10-ml-openapi.yml
  format: yaml
  label: Windows ML API
  slug: windows-ml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-ml-openapi.yml
- filename: microsoft-windows-10-storage-openapi.yml
  format: yaml
  label: Windows Storage API
  slug: windows-storage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-storage-openapi.yml
- filename: microsoft-windows-10-cortana-openapi.yml
  format: yaml
  label: Windows Cortana API
  slug: windows-cortana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-cortana-openapi.yml
- filename: microsoft-windows-10-ink-openapi.yml
  format: yaml
  label: Windows Ink API
  slug: windows-ink-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-ink-openapi.yml
- filename: microsoft-windows-10-composition-openapi.yml
  format: yaml
  label: Windows Composition API
  slug: windows-composition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-composition-openapi.yml
- filename: microsoft-windows-10-directx-openapi.yml
  format: yaml
  label: DirectX Graphics API
  slug: directx-graphics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-directx-openapi.yml
- filename: microsoft-windows-10-media-capture-openapi.yml
  format: yaml
  label: Windows Media Capture API
  slug: windows-media-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-media-capture-openapi.yml
- filename: microsoft-windows-10-networking-openapi.yml
  format: yaml
  label: Windows Networking API
  slug: windows-networking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-networking-openapi.yml
- filename: microsoft-windows-10-bluetooth-openapi.yml
  format: yaml
  label: Windows Bluetooth API
  slug: windows-bluetooth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-bluetooth-openapi.yml
- filename: microsoft-windows-10-geolocation-openapi.yml
  format: yaml
  label: Windows Geolocation API
  slug: windows-geolocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-geolocation-openapi.yml
- filename: microsoft-windows-10-sensors-openapi.yml
  format: yaml
  label: Windows Sensors API
  slug: windows-sensors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-sensors-openapi.yml
- filename: microsoft-windows-10-hello-openapi.yml
  format: yaml
  label: Windows Hello Authentication API
  slug: windows-hello-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-hello-openapi.yml
- filename: microsoft-windows-10-winui-openapi.yml
  format: yaml
  label: WinUI API
  slug: winui-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-winui-openapi.yml
- filename: microsoft-windows-10-background-tasks-openapi.yml
  format: yaml
  label: Windows Background Tasks API
  slug: windows-background-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/openapi/microsoft-windows-10-background-tasks-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Nov 20 02:11:36 2026 GMT
  host: developer.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Windows 10 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Windows 10, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Windows 10
provider_slug: microsoft-windows-10
slug: microsoft-windows-10-domain-security
source_filename: microsoft-windows-10-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 02:11:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-10/refs/heads/main/security/microsoft-windows-10-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Desktop
- Operating System
- UWP
- Win32
- Windows
---
