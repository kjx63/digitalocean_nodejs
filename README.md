# digitalocean_nodejs

After making changes to the git repository...

(This is the link to deploy your node.js app to the digital ocean server first time)
https://www.youtube.com/watch?v=oykl1Ih9pMg&lc=UgypQGihGEhMd_N419p4AaABAg.9-DtDYG9dPg9AR2oV-SgU8&feature=em-comments


MacBook-Pro:~ kenjiueyama$ ssh root@ip_address


root@node-app:~# ls

apps  menkyo-v2


root@node-app:~# cd apps/

root@node-app:~/apps# 


root@node-app:~/apps# ls

empty 

root@node-app:~/apps# git clone https://github.com/kjx63...

root@node-app:~/apps# ls

menkyo-v2


root@node-app:~/apps# cd menkyo-v2/


root@node-app:~/apps/menkyo-v2# ls
app.js  node_modules       package.json  routes
bin     package-lock.json  public        views

root@node-app:~/apps/menkyo-v2# pm2 stop app.js 

[PM2] Applying action stopProcessId on app [app.js](ids: [ 0 ])
[PM2] [app](0) ✓
┌────┬────────────────────┬──────────┬──────┬───────────┬──────────┬──────────┐
│ id │ name               │ mode     │ ↺    │ status    │ cpu      │ memory   │
├────┼────────────────────┼──────────┼──────┼───────────┼──────────┼──────────┤
│ 0  │ app                │ fork     │ 0    │ stopped   │ 0%       │ 0b       │
└────┴────────────────────┴──────────┴──────┴───────────┴──────────┴──────────┘

root@node-app:~/apps/menkyo-v2# pm2 start app.js 

[PM2] Applying action restartProcessId on app [app](ids: [ 0 ])
[PM2] [app](0) ✓
[PM2] Process successfully started
┌────┬────────────────────┬──────────┬──────┬───────────┬──────────┬──────────┐
│ id │ name               │ mode     │ ↺    │ status    │ cpu      │ memory   │
├────┼────────────────────┼──────────┼──────┼───────────┼──────────┼──────────┤
│ 0  │ app                │ fork     │ 0    │ online    │ 0%       │ 19.8mb   │
└────┴────────────────────┴──────────┴──────┴───────────┴──────────┴──────────┘


