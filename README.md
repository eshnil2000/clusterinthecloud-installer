# Cluster in the Cloud

Heterogenerous, scalable compute clusters in the cloud.

## Installer script

Requirements:
- Python >= 2.7
- `ssh`, `ssh-keygen` and `scp`

## Changes required in install-citc.py: 
    parser.add_argument("--terraform-repo", default="eshnil2000/clusterinthecloud-terraform", help="CitC Terraform GitHub project repo to use")
    #parser.add_argument("--terraform-repo", default="clusterinthecloud/terraform", help="CitC Terraform GitHub project repo to use")
   
    os.rename("clusterinthecloud-terraform-{branch}".format(branch=args.terraform_branch), "citc-terraform")
    #os.rename("terraform-{branch}".format(branch=args.terraform_branch), "citc-terraform")
