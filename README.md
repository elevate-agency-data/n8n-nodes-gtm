# n8n-nodes-gtm  

This is an n8n community node. It lets you interact with Google Tag Manager (GTM) in your n8n workflows.  

Google Tag Manager is a tag management system that allows users to quickly and easily update tags and code snippets on their websites or mobile apps.  

[n8n](https://n8n.io/) is a [fair-code licensed](https://docs.n8n.io/reference/license/) workflow automation platform.  

[Installation](#installation)  
[Credentials](#credentials)    
[Operations](#operations)   
[Compatibility](#compatibility)   
[Usage](#usage)  
[Resources](#resources)  

## Installation  

Follow the [installation guide](https://docs.n8n.io/integrations/community-nodes/installation/) in the n8n community nodes documentation.  

Alternatively, you can manually install it:  

```sh  
git clone https://github.com/elevate-agency-data/n8n-nodes-gtm.git 
cd n8n-nodes-gtm 
npm install  
```  

Then, place the node file in the `~/.n8n/custom-nodes` directory (or follow instructions specific to your n8n installation).   

## Credentials  

To use this node, you need a Google Cloud API key with access to Google Tag Manager.  

## Operations  

This node supports the following operations within Google Tag Manager:  

* **Account**
    - Gets an account
    - List all accounts
    - Updates an account
* **Built-In Variable**
    - Create a built-in variable
    - Delete a built-in variable
    - Lists all the enabled built-in variables
    - Reverts changes to a built-in variable
* **Client**
    - Creates a client
    - Deletes a client
    - Gets a client
    - Lists all clients
    - Reverts changes to a client
    - Updates a client
* **Container**
    - Combines containers
    - Creates a container
    - Deletes a container
    - Gets a container
    - Lists all containers
    - Looks up a container
    - Move tag ID out of a container
    - Gets the tagging snippet for a container
    - Updates a container
* **Destination**
    - Gets a destination
    - Adds a destination
    - Lists all destinations
* **Environment**
    - Creates an environment
    - Deletes an environment
    - Gets an environment
    - Lists all environments
    - Re-generates the authorization code for an environment
    - Updates an environment
* **Folder**
    - Creates a folder
    - Deletes a folder
    - List all entities in a folder
    - Gets a folder
    - Lists all folders
    - Moves entities to a folder
    - Reverts changes to a folder
    - Updates a folder
* **Google Tag Configuration**
    - Creates a google tag config
    - Deletes a google tag config
    - Gets a google tag config
    - Lists all google tag configs
    - Updates a google tag config
* **Tag**
    - Creates a tag
    - Deletes a tag
    - Gets a tag
    - Lists all tags
    - Reverts changes to a tag
    - Updates a tag
* **Template**
    - Creates a custom template
    - Deletes a template
    - Gets a template
    - Imports a template from gallery
    - Lists all templates
    - Reverts changes to a template
    - Updates a templates
* **Transformation**
    - Creates a transformation
    - Deletes a transformation
    - Gets a transformation
    - Lists all transformations
    - Reverts changes to a transformation
    - Updates a transformation
* **Trigger**
    - Creates a trigger
    - Deletes a trigger
    - Gets a trigger
    - Lists all triggers
    - Reverts changes to a trigger
    - Updates a trigger
* **User Permission**
    - Creates a user's permissions
    - Remove a user's permissions
    - Gets a user's permissions
    - Lists all users that have access
    - Updates a user's permissions
* **Variable**
    - Creates a variable
    - Deletes a variable
    - Gets a variable
    - Lists all variables
    - Reverts changes to a variable
    - Updates a variable
* **Version Header**
    - Gets the latest container version header
    - Lists all container versions
* **Version**
    - Deletes a version
    - Gets a version
    - Gets the live version
    - Publishes a version
    - Sets the latest versions
    - Undeletes a version
    - Updates a version
* **Workspace**
    - Creates a workspace
    - Creates a container version from the entities present in the workspace
    - Deletes a workspace
    - Finds conflicting and modified entities in the workspace
    - Gets a workspace
    - Lists all workspaces
    - Quick previews a workspace
    - Resolves a merge conflict for a workspace entity
    - Syncs a workspace to the latest container version
    - Updates a workspace
* **Zone**
    - Creates a zone
    - Deletes a zone
    - Gets a zone
    - Lists all zones
    - Reverts changes to a zone
    - Updates a zone

Retrieve information from the [GTM API](https://developers.google.com/tag-platform/tag-manager/api/v2?hl=fr). 

### Steps to obtain API credentials:  

1. Go to the [Google Cloud Console](https://console.cloud.google.com/)  
2. Create a new project or use an existing one  
3. Enable the **Google Tag Manager API**  
4. Create API credentials (API key or OAuth 2.0)  
5. Add your API key to the authentication settings in n8n  

## Compatibility  

- Tested with: 1.80.5 (Success)

## Usage  

Once installed and configured, this node can be used in n8n workflows to automate GTM operations such as managing containers, updating tags, and tracking real-time changes.  

## Resources  

- [n8n community nodes documentation](https://docs.n8n.io/integrations/community-nodes/)  
- [Google Tag Manager API documentation](https://developers.google.com/tag-platform/tag-manager/api/v2)