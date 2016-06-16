# What is Authorization?  
Authorization is the process of determining what permissions someone has to perform specific actions within an application. 

Once a user has entered in a valid login and password (authentication), there are the permission checks (authorization) that are performed to specify what they have access to in your system. 

Think of it this way:  You have tickets to a baseball game. They check your ticket at the gate to authenticate that you have valid credentials to enter the stadium. Once you’re inside, your ticket also dictates what seat you are in and authorizes you to access that section of the stadium. 

## Structuring  a User Directory 
The ability to set authorization permissions is based off your segments of users. First things first, let’s talk about your options for structuring your user database. 

### Users
Users are the individual people accessing your applications who have valid account credentials. 

### Groups
Groups are a collection of users that are tied together based on a specific purpose. For example, you could have groups of admins that can access all facets of your application and control permissions. Users could belong to more than one group. 

### Roles
Roles are predetermined permissions based on a user’s specific function within your application. For example, you may want your admins to be able to publish changes to your application whereas a different group of users should only be able to make edits. 

# Types of Authorization

## Simple Authorization 
Simple authorization involves hard-coding permission checks into your application and assigning them to a user or group.

*Pros:* The basic logic is easy to build and sufficient for applications with smaller user databases. 
*Cons:* Difficult to change authorization rules dynamically and can require a lot of refactoring. 

## Permission-Based Authorization 

Permission-based authorization is a more dynamic way of handling authorization. Permissions are statements of functionality that define and resource and what actions it can perform. Permission-based authorization separates your application logic from your data model. 

*Pros:* Easy to change authorization rules dynamically and provides flexibility to your security model. 
*Cons:* Difficult to change authorization rules dynamically and can require a lot of refactoring. 

# How to Setup Access Control 

## Fine-Grained Permissions
Fine-grained permissions allow you to control user access based on activity, state, or unique attributes. These permissions are custom logic that you write  specifically for your application. They can either add flexibility to your group or role authorization, or replace it all together. Fine-grained permissions are based on filters of user data parameters. 
