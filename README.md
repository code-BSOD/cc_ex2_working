1. After modifying all 3 code files, need to build it locally and test.

2. Then push it to docker hub

3. In VM, copy the docker-compose.yml file and remove the build tag or comment it

4. Using `sudo docker-compose up` would run the application.

5. Before running step 4, create a Firewall rule with Source IP Range `0.0.0.0/0` and with TCP Port `4243,3000` enabled.

6. Edit the `docker.service` file as mentioned in the instructions and add the missing `-H tcp://0.0.0.0:4243` to it.

7. Then restart the Daemon and Docker engine according to instructions

8. Run step 4 now.

9. Should be able to run the app and submit it without any issue.