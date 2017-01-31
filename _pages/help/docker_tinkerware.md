---
resource: true
categories: Help
title: TinkerWare works with Docker too.
---

# Don't Repeat Yourself. TinkerWare works with Docker too.

### Building, Maintaining, Deploying Containers

## Complexity does NOT dissappear

A container doesn't consume complexity and emit order. The complexity is still in there; 
you still have to build your containers in a way that is replicable, reliable, and automatable.

In many cases some of the complexity is now being outsourced to others who maintain the containers.
When there are system level changes and patching, we have to make sure every container up to date and
create a new image once again to have the immutable infrastructure.

Of course it's easier to deploy new features to a container. But before that we need to deploy 
the containers and setup an evironment to start mounting our applications. These tasks that can be automated and documented.

Let's say you have the containers. Now you want to deploy test and production environments.
How do containers know which environment they're running in? Or specifically, 
things like what's the database user/password, what queue to connect to, where to find local 
endpoint for service X? 

That still needs to live outside containers. 

### TinkerWare

Here's where TinkerWare comes in. There's always a point where what you're doing is unique 
to your environment, and you have to be able to manage/reproduce/upgrade it somehow.

We provide a platform where users can select the automated tools ready to apply to a Docker container,
and keep track of your infrastructure in a documented and fully functional way.
View [Infrastructure as code](https://en.wikipedia.org/wiki/Infrastructure_as_Code)

Benefits:
  - Manage, scale and track your projects. The one that use Docker and the ones that doesn't
  - Work locally with docker if needed.
  - Deploy automatically even if you use docker.
    * A fully tested environment won't fail if it is replicated.
    * The local environment would act as the production env. That way you know it's working
    * On a clean server we take care of installing docker and mounting everything as you defined
    on your configurations using our platform. 
  - Integrate easily new features, or even new containers to your infrastructure.
  - Recover faster from failures with your documented configs
  - Easier to extend and maintain
  

The docker provisioner is ideal for organizations that are using Docker 
as a means to distribute things like their application or services. 

In a few words, once more: 
   `Tinkerware wants the users to define their own architecture. We just make that faster and easier`
Speaking about Docker specifically, we setup containers based on your defined configurations.

## Credits and references.

1. [Hacker News YCombinator](https://news.ycombinator.com/item?id=11963268)
