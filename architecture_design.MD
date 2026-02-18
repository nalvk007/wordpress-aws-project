                        Internet
                            |
                     ----------------
                     |              |
               Security Group   Security Group
                     |              |
                EC2 - PROD      EC2 - DEV
              (Apache + PHP)  (Apache + PHP)
              (Local MySQL)   (Local MySQL)
                     |
               CloudWatch
                - Metrics
                - Alarms
                - Logs

Dev Instance:
EventBridge Scheduler
  -> Start 9 AM
  -> Stop 6 PM

