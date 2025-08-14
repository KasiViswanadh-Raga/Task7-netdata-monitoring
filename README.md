# Netdata System Monitoring (Task 7)

*Objective:* Install Netdata via Docker and visualize system/app performance metrics.  
*Tools:* Netdata, Docker

## Steps I followed
1. Pulled and ran the Netdata container:
   bash
   docker run -d --name=netdata -p 19999:19999 netdata/netdata

2. Accessed the dashboard at http://localhost:19999.


3. Monitored CPU, Memory, Disk, and Docker metrics.


4. Checked logs in /var/log/netdata:

docker exec -it netdata sh
ls /var/log/netdata
cat /var/log/netdata/error.log
exit


5. Captured the dashboard screenshot.



Screenshot



Notes

To stop/remove Netdata:

docker stop netdata && docker rm netdata


---

### **⿣ Commit & Push**
In Git Bash:
bash
cd ~/task7-netdata-monitoring
git add README.md dashboard.png
git commit -m "Task 7: Added Netdata dashboard screenshot and README"
git push origin main
