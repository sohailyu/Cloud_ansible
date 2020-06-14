create-efs
=========

This role creates a new EFS volume in AWS.

Requirements
------------

None

Role Variables
--------------

REGION - AWS region to create the EFS volume in.
ENVIRONMENT - The name of the VPC to create the EFS volume in.
PROJECT - The project the EFS volume is going to be used for.
SUBNET_NAME - The subnet tier the EFS volume is to have access to. (i.e. generic)

Dependencies
------------

VPC and subnet exist.

Example Playbook
----------------

		---
		
		- hosts: localhost
		  connection: local
		  gather_facts: False
		  roles:
		    - create-efs

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
