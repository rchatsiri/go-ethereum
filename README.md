#Go-Ethereum

## Resources 
	* Nested VMs Create on Google Cloud: 
		```gcloud compute images create nested-virt \
  		--source-image-project=ubuntu-os-cloud \
  		--source-image-family=ubuntu-1604-lts \
  		--licenses="https://www.googleapis.com/compute/v1/projects/vm-options/global/licenses/enable-vmx"

		gcloud compute instances create "eth-miner-03" --zone "asia-east1-a" --machine-type \
  		"n1-standard-2"  --min-cpu-platform "Intel Haswell" --image "nested-virt-debianv9" \
  		--boot-disk-size "50" --boot-disk-type "pd-ssd" --boot-disk-device-name "geth-nest-disk-00"
		```
