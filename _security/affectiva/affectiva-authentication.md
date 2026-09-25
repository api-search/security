---
anonymous_access: false
api_key_in: []
api_specs:
- filename: affectiva-annotations-api-openapi.yml
  format: yaml
  label: Affectiva Annotations API
  slug: affectiva-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-annotations-api-openapi.yml
- filename: affectiva-data-collection-projects-api-openapi.yml
  format: yaml
  label: Affectiva data collection projects API
  slug: affectiva-data-collection-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-data-collection-projects-api-openapi.yml
- filename: affectiva-entries-api-openapi.yml
  format: yaml
  label: Affectiva Entries API
  slug: affectiva-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-entries-api-openapi.yml
- filename: affectiva-event-configs-api-openapi.yml
  format: yaml
  label: Affectiva event configs API
  slug: affectiva-event-configs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-event-configs-api-openapi.yml
- filename: affectiva-event-instances-api-openapi.yml
  format: yaml
  label: Affectiva event instances API
  slug: affectiva-event-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-event-instances-api-openapi.yml
- filename: affectiva-frame-sampling-jobs-api-openapi.yml
  format: yaml
  label: Affectiva frame sampling jobs API
  slug: affectiva-frame-sampling-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-frame-sampling-jobs-api-openapi.yml
- filename: affectiva-jobs-api-openapi.yml
  format: yaml
  label: Affectiva Jobs API
  slug: affectiva-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-jobs-api-openapi.yml
- filename: affectiva-labeling-job-annotations-api-openapi.yml
  format: yaml
  label: Affectiva Labeling Job Annotations API
  slug: affectiva-labeling-job-annotations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-labeling-job-annotations-api-openapi.yml
- filename: affectiva-labeling-jobs-api-openapi.yml
  format: yaml
  label: Affectiva Labeling Jobs API
  slug: affectiva-labeling-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-labeling-jobs-api-openapi.yml
- filename: affectiva-labeling-tasks-api-openapi.yml
  format: yaml
  label: Affectiva Labeling Tasks API
  slug: affectiva-labeling-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-labeling-tasks-api-openapi.yml
- filename: affectiva-representation-storages-api-openapi.yml
  format: yaml
  label: Affectiva representation storages API
  slug: affectiva-representation-storages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-representation-storages-api-openapi.yml
- filename: affectiva-representations-api-openapi.yml
  format: yaml
  label: Affectiva Representations API
  slug: affectiva-representations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-representations-api-openapi.yml
- filename: affectiva-video-frames-api-openapi.yml
  format: yaml
  label: Affectiva Video Frames API
  slug: affectiva-video-frames-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-video-frames-api-openapi.yml
- filename: affectiva-video-segments-api-openapi.yml
  format: yaml
  label: Affectiva Video Segments API
  slug: affectiva-video-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/openapi/affectiva-video-segments-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Affectiva Authentication
name_suffix: Authentication
oauth_flows: []
overview: Affectiva secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Affectiva
provider_slug: affectiva
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/affectiva-eaas-data_collection_projects.json
  - openapi/affectiva-eaas-entries.json
  - openapi/affectiva-eaas-event_configs.json
  - openapi/affectiva-eaas-event_instances.json
  - openapi/affectiva-eaas-frame_sampling_jobs.json
  - openapi/affectiva-eaas-jobs.json
  - openapi/affectiva-eaas-labeling_job_annotations.json
  - openapi/affectiva-eaas-labeling_jobs.json
  - openapi/affectiva-eaas-labeling_tasks.json
  - openapi/affectiva-eaas-representation_storages.json
  - openapi/affectiva-eaas-representations.json
  - openapi/affectiva-eaas-video_frames.json
  - openapi/affectiva-eaas-video_segments.json
  type: http
slug: affectiva-authentication
source_filename: affectiva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: openapi/affectiva-eaas-data_collection_projects.json, openapi/affectiva-eaas-entries.json, openapi/affectiva-eaas-event_configs.json,\n  openapi/affectiva-eaas-event_instances.json, openapi/affectiva-eaas-frame_sampling_jobs.json, openapi/affectiva-eaas-jobs.json,\n  openapi/affectiva-eaas-labeling_job_annotations.json, openapi/affectiva-eaas-labeling_jobs.json, openapi/affectiva-eaas-labeling_tasks.json,\n  openapi/affectiva-eaas-representation_storages.json, openapi/affectiva-eaas-representations.json, openapi/affectiva-eaas-video_frames.json\n  ... + live 401 challenge from https://index.affectiva.com/jobs\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/affectiva-eaas-data_collection_projects.json\n  - openapi/affectiva-eaas-entries.json\n  - openapi/affectiva-eaas-event_configs.json\n  - openapi/affectiva-eaas-event_instances.json\n  - openapi/affectiva-eaas-frame_sampling_jobs.json\n\
  \  - openapi/affectiva-eaas-jobs.json\n  - openapi/affectiva-eaas-labeling_job_annotations.json\n  - openapi/affectiva-eaas-labeling_jobs.json\n  - openapi/affectiva-eaas-labeling_tasks.json\n  - openapi/affectiva-eaas-representation_storages.json\n  - openapi/affectiva-eaas-representations.json\n  - openapi/affectiva-eaas-video_frames.json\n  - openapi/affectiva-eaas-video_segments.json\nobserved:\n  url: https://index.affectiva.com/jobs\n  http_status: 401\n  www_authenticate: Basic realm=\"Affectiva Facial Coding API\"\n  body: '{\"error\":\"Please login to continue.\"}'\n  fetched: '2026-09-12'\n  note: 'The live API confirms the contract: HTTP Basic across the whole surface, one realm, no bearer\n    token, no API key header and no OAuth. This probe is also the OWNERSHIP proof for the spec set — the\n    realm string names Affectiva explicitly on a host in Affectiva''s own registrable domain.'\ngaps:\n- No operation in any of the thirteen documents declares a 401 or 403 response,\
  \ despite blanket enforcement.\n- No scopes, roles or permissions surface exists — HTTP Basic carries no authorization model.\n- Credentials are issued by sales; https://index.affectiva.com/users/sign_up returns 404.\n- 'No public authentication documentation page: knowledge.affectiva.com returns a readme.io \"Not Yet Active\"\n  placeholder (401) and developer.affectiva.com 302s to an Atlassian login.'\nconsole:\n  url: https://index.affectiva.com/users/sign_in\n  http_status: 200\n  branding: The sign-in page is branded \"iMotions Developer Platform\" — iMotions is the Smart Eye sibling\n    brand Affectiva's product line was folded into.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/affectiva/refs/heads/main/authentication/affectiva-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Emotion AI
- Artificial Intelligence
- Machine Learning
- Computer Vision
- Facial Coding
- Facial Expression Analysis
- Media Analytics
- Market Research
- Automotive
- Driver Monitoring
- Video Analysis
- Affective Computing
---
