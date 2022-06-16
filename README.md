# connector-playbook-automation
Playbook Automation:

-Input Parameters: 
	
	--connector_info : Path of connector's info.json file.
	--output : Output directory location. (default is current directory)

-Result: 

	Creates sample playbook collection JSON file.

-Usage:

    - This script(generate_sample_playbook.py) generates new sample playbook collection, required to ship with connector.    
    - Python package dependency configparser==3.5.0.
    - Script generates a sample playbook collection, consists of playbook for each connector action. Resulted filename will be "Sample - <CONNECTOR NAME - CONNECTOR.VERSION>.json".
    - User need to modify the sample playbooks manually to specify desired default value in the connector step of playbook.
    - User can import the sample playbook collection into CyOPs.
    - Refer following example.
        python generate_sample_playbook.py --connector_info info.json --output /home/user/playbooks/
