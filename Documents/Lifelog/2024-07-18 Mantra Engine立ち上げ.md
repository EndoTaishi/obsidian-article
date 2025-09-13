``` zsh
~ on ☁️  (ap-northeast-1) 
at 17:12:14 ❯ cd Documents/GitHub/mantra/mantra-engine-client 

mantra-engine-client on main [✔️] via  v18.20.4 on ☁️  (ap-northeast-1) 
at 17:12:29 ❯ npm run serve

> mantra_editor@34.0.0 serve
> vite dev


  VITE v5.1.7  ready in 840 ms

  ➜  Local:   http://localhost:8080/
  ➜  Network: use --host to expose
  ➜  press h + enter to show help
5:16:17 PM [vite] .env.development.local changed, restarting server...
5:16:17 PM [vite] .env.development.local changed, restarting server... (x2)
5:16:17 PM [vite] server restarted.
5:16:25 PM [vite] .env.development.local changed, restarting server...
5:16:25 PM [vite] server restarted.

```

# API
``` zsh
~ on ☁️  (ap-northeast-1) 
at 17:07:35 ❯ cd Documents/GitHub/mantra/mantra-engine-api 

mantra-engine-api on main [✔️] via 🐳 desktop-linux via  v18.20.4 via 🐍v3.12.4 on ☁️  (ap-northeast-1) 
at 17:07:47 ❯ bash create_env.sh remote_db_test > config/settings/.env

mantra-engine-api on main [✔️] via 🐳 desktop-linux via  v18.20.4 via 🐍v3.12.4 on ☁️  (ap-northeast-1) 
at 17:08:14 ❯ export REMOTE_DB_HOST=mantra-engine-test2-cluster.cluster-ckivu92qyn9a.ap-northeast-1.rds.amazonaws.com


mantra-engine-api on main [✔️] via 🐳 desktop-linux via  v18.20.4 via 🐍v3.12.4 on ☁️  (ap-northeast-1) 
at 17:08:27 ❯ docker-compose up
WARN[0000] /Users/endotaishi/Documents/GitHub/mantra/mantra-engine-api/docker-compose.yml: `version` is obsolete 
[+] Building 44.2s (15/15) FINISHED                                  docker:desktop-linux
 => [db-tunnel internal] load build definition from Dockerfile_tunnel                0.0s
 => => transferring dockerfile: 984B                                                 0.0s
 => [db-tunnel internal] load metadata for docker.io/library/ubuntu:22.04            2.4s
 => [db-tunnel auth] library/ubuntu:pull token for registry-1.docker.io              0.0s
 => [db-tunnel internal] load .dockerignore                                          0.0s
 => => transferring context: 65B                                                     0.0s
 => [db-tunnel  1/10] FROM docker.io/library/ubuntu:22.04@sha256:340d9b015b194dc6e2  1.8s
 => => resolve docker.io/library/ubuntu:22.04@sha256:340d9b015b194dc6e2a13938944e0d  0.0s
 => => sha256:3713021b02770a720dea9b54c03d0ed83e03a2ef5dce2898c56 29.53MB / 29.53MB  1.1s
 => => sha256:340d9b015b194dc6e2a13938944e0d016e57b9679963fdeb9ce02 1.13kB / 1.13kB  0.0s
 => => sha256:0eb0f877e1c869a300c442c41120e778db7161419244ee5cbc6fa5f13 424B / 424B  0.0s
 => => sha256:8a3cdc4d1ad3e314a91f76b7b99eed443f2152e3a9bf33e46669b 2.30kB / 2.30kB  0.0s
 => => extracting sha256:3713021b02770a720dea9b54c03d0ed83e03a2ef5dce2898c56a327fee  0.6s
 => [db-tunnel  2/10] RUN apt-get update && apt-get install -y curl unzip socat ne  30.3s
 => [db-tunnel  3/10] RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_6  2.9s 
 => [db-tunnel  4/10] RUN unzip awscliv2.zip                                         1.6s 
 => [db-tunnel  5/10] RUN ./aws/install                                              0.9s 
 => [db-tunnel  6/10] RUN rm awscliv2.zip                                            0.1s 
 => [db-tunnel  7/10] RUN rm -rf aws/                                                0.2s 
 => [db-tunnel  8/10] RUN curl "https://s3.amazonaws.com/session-manager-downloads/  2.9s 
 => [db-tunnel  9/10] RUN dpkg -i session-manager-plugin.deb                         0.3s 
 => [db-tunnel 10/10] RUN rm session-manager-plugin.deb                              0.1s 
 => [db-tunnel] exporting to image                                                   0.5s 
 => => exporting layers                                                              0.5s 
 => => writing image sha256:bf9fc19ea68a5042aab9264316b159ac1cdcd486d423df7ce655512  0.0s 
 => => naming to docker.io/library/mantra-engine-api-db-tunnel                       0.0s 
[+] Running 3/3                                                                           
 ✔ Network mantra-engine-api_container-network  Created                              0.0s 
 ✔ Container mantra-engine-api-db-tunnel-1      Created                              0.0s 
 ✔ Container mantraengine_api                   Crea...                              0.5s 
Attaching to db-tunnel-1, mantraengine_api
db-tunnel-1       | 
db-tunnel-1       | Starting session with SessionId: taishi-vub243mfgckkgqs6yc76jxnsc4
db-tunnel-1       | Port 3306 opened for sessionId taishi-vub243mfgckkgqs6yc76jxnsc4.
db-tunnel-1       | Waiting for connections...
db-tunnel-1       | 
db-tunnel-1       | Connection accepted for session [taishi-vub243mfgckkgqs6yc76jxnsc4]
mantraengine_api  | [2024/07/17 17:10:18] INFO django.utils.autoreload run_with_reloader():668 - Watching for file changes with StatReloader
mantraengine_api  | [2024/07/17 17:13:48] WARNING django.request log_response():241 - Not Found: /
mantraengine_api  | [2024/07/17 17:13:48] WARNING django.server log_message():212 - "GET / HTTP/1.1" 404 2649
mantraengine_api  | [2024/07/17 17:13:48] WARNING django.request log_response():241 - Not Found: /favicon.ico
mantraengine_api  | [2024/07/17 17:13:48] WARNING django.server log_message():212 - "GET /favicon.ico HTTP/1.1" 404 2700
mantraengine_api  | [2024/07/17 17:13:50] WARNING django.request log_response():241 - Not Found: /
mantraengine_api  | [2024/07/17 17:13:50] WARNING django.server log_message():212 - "GET / HTTP/1.1" 404 2649
mantraengine_api  | [2024/07/17 17:14:21] INFO django.server log_message():212 - "OPTIONS /api/graphql/ HTTP/1.1" 200 0
mantraengine_api  | [2024/07/17 17:14:21] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 606
mantraengine_api  | [2024/07/17 17:14:21] INFO django.server log_message():212 - "OPTIONS /api/tags/ HTTP/1.1" 200 0
mantraengine_api  | [2024/07/17 17:14:21] INFO django.server log_message():212 - "OPTIONS /api/usertypes/? HTTP/1.1" 200 0
mantraengine_api  | [2024/07/17 17:14:22] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 107
mantraengine_api  | [2024/07/17 17:14:22] INFO django.server log_message():212 - "GET /api/usertypes/? HTTP/1.1" 200 205
mantraengine_api  | [2024/07/17 17:14:22] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 79
mantraengine_api  | [2024/07/17 17:14:22] INFO django.server log_message():212 - "GET /api/tags/ HTTP/1.1" 200 2
mantraengine_api  | [2024/07/17 17:14:22] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 75
mantraengine_api  | [2024/07/17 17:15:48] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 606
mantraengine_api  | [2024/07/17 17:15:48] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 480
mantraengine_api  | [2024/07/17 17:15:48] INFO django.server log_message():212 - "GET /api/tags/ HTTP/1.1" 200 2
mantraengine_api  | [2024/07/17 17:15:48] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 79
mantraengine_api  | [2024/07/17 17:15:48] INFO django.server log_message():212 - "GET /api/usertypes/? HTTP/1.1" 200 205
mantraengine_api  | [2024/07/17 17:15:48] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 890
mantraengine_api  | [2024/07/17 17:17:43] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 606
mantraengine_api  | [2024/07/17 17:17:43] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 480
mantraengine_api  | [2024/07/17 17:17:43] INFO django.server log_message():212 - "GET /api/tags/ HTTP/1.1" 200 2
mantraengine_api  | [2024/07/17 17:17:43] INFO django.server log_message():212 - "GET /api/usertypes/? HTTP/1.1" 200 205
mantraengine_api  | [2024/07/17 17:17:43] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 79
mantraengine_api  | [2024/07/17 17:17:44] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 890
mantraengine_api  | [2024/07/17 18:05:13] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 606
mantraengine_api  | [2024/07/17 18:05:13] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 480
mantraengine_api  | [2024/07/17 18:05:13] INFO django.server log_message():212 - "GET /api/tags/ HTTP/1.1" 200 2
mantraengine_api  | [2024/07/17 18:05:14] INFO django.server log_message():212 - "GET /api/usertypes/? HTTP/1.1" 200 205
mantraengine_api  | [2024/07/17 18:05:14] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 79
mantraengine_api  | [2024/07/17 18:05:14] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 890
mantraengine_api  | [2024/07/17 18:05:17] INFO django.server log_message():212 - "OPTIONS /api/chapters/1055/ HTTP/1.1" 200 0
mantraengine_api  | [2024/07/17 18:05:17] INFO pfadmin.serializer get_display_translation_engine():339 - gpt4
mantraengine_api  | [2024/07/17 18:05:17] INFO pfadmin.serializer get_display_translation_engine():340 - {'skip_ocr': False, 'use_gpt4': True, 'bubble_style': {}, 'default_style': {}, 'set_default_style': False, 'automatic_typesetting': True, 'empty_machine_translation': False}
mantraengine_api  | [2024/07/17 18:05:17] INFO django.server log_message():212 - "GET /api/chapters/1055/ HTTP/1.1" 200 905
mantraengine_api  | [2024/07/17 18:05:18] INFO django.server log_message():212 - "GET /api/tags/ HTTP/1.1" 200 2
mantraengine_api  | [2024/07/17 18:05:18] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 11074
mantraengine_api  | [2024/07/17 18:05:23] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 11074
mantraengine_api  | [2024/07/17 18:05:29] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 11074
mantraengine_api  | [2024/07/17 18:05:34] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 11074
mantraengine_api  | [2024/07/17 18:05:40] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 11074
mantraengine_api  | [2024/07/17 18:05:40] INFO django.server log_message():212 - "GET /api/usertypes/? HTTP/1.1" 200 205
mantraengine_api  | [2024/07/17 18:05:40] INFO django.server log_message():212 - "GET /api/tags/ HTTP/1.1" 200 2
mantraengine_api  | [2024/07/17 18:05:40] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 79
mantraengine_api  | [2024/07/17 18:05:41] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 890
mantraengine_api  | [2024/07/17 18:05:47] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 375
mantraengine_api  | [2024/07/17 18:05:47] INFO django.server log_message():212 - "OPTIONS /api/books/745/assignments/ HTTP/1.1" 200 0
mantraengine_api  | [2024/07/17 18:05:48] INFO django.server log_message():212 - "GET /api/books/745/assignments/ HTTP/1.1" 200 33
mantraengine_api  | [2024/07/17 18:05:48] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 257
mantraengine_api  | [2024/07/17 18:05:49] INFO django.server log_message():212 - "GET /api/usertypes/? HTTP/1.1" 200 205
mantraengine_api  | [2024/07/17 18:05:49] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 79
mantraengine_api  | [2024/07/17 18:05:50] INFO django.server log_message():212 - "GET /api/tags/ HTTP/1.1" 200 2
mantraengine_api  | [2024/07/17 18:05:50] INFO django.server log_message():212 - "POST /api/graphql/ HTTP/1.1" 200 890
mantraengine_api  | [2024/07/17 18:08:14] INFO django.server log_message():212 - "GET /kanrigamen/pfadmin HTTP/1.1" 302 0
mantraengine_api  | [2024/07/17 18:08:14] INFO django.server log_message():212 - "GET /kanrigamen/login/?next=/kanrigamen/pfadmin HTTP/1.1" 200 4228
mantraengine_api  | [2024/07/17 18:08:14] INFO django.server log_message():212 - "GET /static/admin/css/dark_mode.css HTTP/1.1" 200 2929
mantraengine_api  | [2024/07/17 18:08:14] INFO django.server log_message():212 - "GET /static/admin/js/theme.js HTTP/1.1" 200 1943
mantraengine_api  | [2024/07/17 18:08:14] INFO django.server log_message():212 - "GET /static/admin/css/responsive.css HTTP/1.1" 200 18559
mantraengine_api  | [2024/07/17 18:08:14] INFO django.server log_message():212 - "GET /static/admin/css/base.css HTTP/1.1" 200 21310
mantraengine_api  | [2024/07/17 18:08:14] INFO django.server log_message():212 - "GET /static/admin/js/nav_sidebar.js HTTP/1.1" 200 3063
mantraengine_api  | [2024/07/17 18:08:14] INFO django.server log_message():212 - "GET /static/admin/css/nav_sidebar.css HTTP/1.1" 200 2694
mantraengine_api  | [2024/07/17 18:08:14] INFO django.server log_message():212 - "GET /static/admin/css/login.css HTTP/1.1" 200 958
Gracefully stopping... (press Ctrl+C again to force)
[+] Stopping 2/2
 ✔ Container mantraengine_api               Stopped                                  0.2s 
 ✔ Container mantra-engine-api-db-tunnel-1  Stopped                                 10.1s 
```

