# 

**[Installation](#installation) 7**

> [Architecture](#architecture) 7
>
> [Release Notes](#release-notes) 7
>
> [Frontend - Home](#frontend---home) 8
>
> [Backend - Home](#backend---home) 8
>
> [Database](#database) 8
>
> [Create Operations](#create-operations) 8
>
> [Read Operations](#read-operations) 9
>
> [Update Operations](#update-operations) 9
>
> [Delete Operations](#delete-operations) 9
>
> [Bulk Write](#bulk-write) 10
>
> [Versioning](#versioning) 10
>
> [Key relevant GitLab
> documentation](#key-relevant-gitlab-documentation) 10
>
> [Popular topics](#popular-topics) 11
>
> [The entire DevOps lifecycle](#the-entire-devops-lifecycle) 12

**[Introduction](#introduction) 12**

> [Helping the community](#helping-the-community) 12
>
> [Communicate better](#communicate-better) 12
>
> [What fields are included in a
> project?](#what-fields-are-included-in-a-project) 12
>
> [What is a Projects Platform?](#what-is-a-projects-platform) 13
>
> [Getting Started](#getting-started) 13
>
> [Our current Projects platform folder
> structure](#our-current-projects-platform-folder-structure) 13
>
> [Key Folders](#key-folders) 13
>
> [Application Dialogs (appdialogs)](#application-dialogs-appdialogs) 13
>
> [Assets (assets)](#assets-assets) 13
>
> [Global Functions (functs)](#global-functions-functs) 13
>
> [Mixins (mixins)](#mixins-mixins) 13
>
> [Mini Pop-in Windows(miniwins)](#mini-pop-in-windowsminiwins) 13
>
> [Pages (pages)](#pages-pages) 13
>
> [Popups (popups)](#popups-popups) 14
>
> [SCSS (scss)](#scss-scss) 14
>
> [Shared Components (shrcomponents)](#shared-components-shrcomponents)
> 14
>
> [Windows (wins)](#windows-wins) 14
>
> [Custom Vue Event Bus (VBUS)](#custom-vue-event-bus-vbus) 14

**[Application & Component Instances](#application-component-instances)
15**

> [Creating an Application Instance](#creating-an-application-instance)
> 15
>
> [\#The Root Component](#the-root-component) 16
>
> [\#Component Instance Properties](#component-instance-properties) 17
>
> [\#Lifecycle Hooks](#lifecycle-hooks) 18
>
> [\#Lifecycle Diagram](#lifecycle-diagram) 19

**[Template Syntax](#template-syntax) 20**

> [\#Interpolations](#interpolations) 20
>
> [\#Text](#text) 20
>
> [\#Raw HTML](#raw-html) 20
>
> [\#Attributes](#attributes) 21
>
> [\#Using JavaScript Expressions](#using-javascript-expressions) 21
>
> [\#Directives](#directives) 22
>
> [\#Arguments](#arguments) 22
>
> [\#Dynamic Arguments](#dynamic-arguments) 22
>
> [\#Modifiers](#modifiers) 23
>
> [\#Shorthands](#shorthands) 23
>
> [\#Caveats](#caveats) 24
>
> [\#Dynamic Argument Value
> Constraints](#dynamic-argument-value-constraints) 24
>
> [\#Dynamic Argument Expression
> Constraints](#dynamic-argument-expression-constraints) 24

**[Data Properties and Methods](#data-properties-and-methods) 25**

> [\#Data Properties](#data-properties) 25
>
> [\#Methods](#methods) 26

**[Computed Properties and Watchers](#computed-properties-and-watchers)
31**

> [\#Computed Properties](#computed-properties) 31
>
> [\#Basic Example](#basic-example) 32
>
> [\#Computed Caching vs Methods](#computed-caching-vs-methods) 33
>
> [\#Computed Setter](#computed-setter) 34
>
> [\#Watchers](#watchers) 35
>
> [\#Computed vs Watched Property](#computed-vs-watched-property) 38

**[Class and Style Bindings](#class-and-style-bindings) 40**

> [\#Binding HTML Classes](#binding-html-classes) 40
>
> [\#Object Syntax](#object-syntax) 40
>
> [\#Array Syntax](#array-syntax) 42
>
> [\#With Components](#with-components) 43
>
> [\#Binding Inline Styles](#binding-inline-styles) 44
>
> [\#Object Syntax](#object-syntax-1) 44
>
> [\#Array Syntax](#array-syntax-1) 45
>
> [\#Auto-prefixing](#auto-prefixing) 45
>
> [\#Multiple Values](#multiple-values) 46

**[Conditional Rendering](#conditional-rendering) 46**

> [\#v-if](#v-if) 46
>
> [\#Conditional Groups with v-if on
> \<template\>](#conditional-groups-with-v-if-on-template) 46
>
> [\#v-else](#v-else) 46
>
> [\#v-else-if](#v-else-if) 47
>
> [\#v-show](#v-show) 47
>
> [\#v-if vs v-show](#v-if-vs-v-show) 47
>
> [\#v-if with v-for](#v-if-with-v-for) 48

**[List Rendering](#list-rendering) 48**

> [\#Mapping an Array to Elements with
> v-for](#mapping-an-array-to-elements-with-v-for) 48
>
> [\#v-for with an Object](#v-for-with-an-object) 49
>
> [\#Maintaining State](#maintaining-state) 50
>
> [\#Array Change Detection](#array-change-detection) 51
>
> [\#Mutation Methods](#mutation-methods) 51
>
> [\#Replacing an Array](#replacing-an-array) 51
>
> [\#Displaying Filtered/Sorted
> Results](#displaying-filteredsorted-results) 52
>
> [\#v-for with a Range](#v-for-with-a-range) 53
>
> [\#v-for on a \<template\>](#v-for-on-a-template) 53
>
> [\#v-for with v-if](#v-for-with-v-if) 54
>
> [\#v-for with a Component](#v-for-with-a-component) 54

**[Shared Components](#shared-components) 57**

> [Admin Sidebar](#admin-sidebar) 57
>
> [Admin Routes (js)](#menu-item-vue) 57
>
> [Admin Sidebar (vue)](#menu-item-vue) 57
>
> [Menu Item (vue)](#menu-item-vue) 57

**[Functions](#functions) 57**

> [API](#functions-js) 57
>
> [Organizations Services (js)](#functions-js) 57
>
> [Types Services (js)](#functions-js) 57
>
> [API services (js)](#functions-js) 58
>
> [Constants (js)](#constants-js) 58
>
> [Dotatlas (js)](#functions-js) 58
>
> [Functions (js)](#functions-js) 59

**[Admin Pages](#admin-pages) 59**

**[Window Components](#window-components) 59**

> [Application Dialogs](#application-dialogs) 59
>
> [Mini Windows](#mini-windows) 59
>
> [Popup Windows](#popup-windows) 59

**[Translation Files](#translation-files) 60**

**[Routing](#routing) 60**

**[Transitions & Animations](#transitions-animations) 60**

**[External Libraries](#external-libraries) 60**

> [Vue.js](#vue.js) 60
>
> [TipTap](#tiptap) 60
>
> [Vue Leaflet](#vue-leaflet) 61
>
> [Vue Color](#vue-color) 61
>
> [Axios](#axios) 61
>
> [Drag and resize](#drag-and-resize) 61
>
> [Bulma](#bulma) 61
>
> [ChartJs](#chartjs) 61

**[State Management](#state-management) 62**

**[Server side Rendering](#server-side-rendering) 62**

# Installation

Currently there are a lot of dependencies required for a Projects
Platform development environment and managing complexity around building
Projects Platform Frontend, Backend, CRI People interface, Sockets etc.
To mitigate the complexity, we decided to build LXC containers to create
a complete environment with all dependencies pre-configured to start
contributing to the Projects Platform code in the shortest possible
time.

We replicate the environmental configuration to build a pre-production
environment too and make an ISO environment for pre-production and
production environment with built-in scripts and access.

1.  Create a [[SSH key]{.ul}](https://www.ssh.com/ssh/key/) and share
    the public key with the core user group member with Projects
    Platform application environment admin access on the main
    development server.

2.  The admin would add the public key in authorized_keys file and would
    create a development environment for the Projects Platform
    application that you would now be able to connect to with the
    provided SSH address *(e.g. : \`ssh dev\@dev.cri-paris.org -p
    :\<\<port\#\>\>\`).*

3.  Access the directory and explore code folders containing frontend
    code at \`/WWW/DEV/FRONT\` or backend code at \`/WWW/DEV/BACK\`.

4.  Install any IDE of your choice and install either SSH tools to
    connect from your computer to the remote server or nautilus
    configuration. (OS dependent)

## Architecture 

The Projects Platform API server is developed in Python using the Flask
micro framework. The data & state of the platform are stored in MongoDB.
Socket.IO server running under python enables real-time, bidirectional
and event-based communication. The client side rendering of DOM of the
Project application leverages VueJS and synchronous interactions are
managed by the socket.io and prosemirror client libraries.

## Release Notes

Latest version: **v0.13.1**

Detailed release notes for each version are available on
[[GitLab]{.ul}](https://git.cri-paris.org/it-team/project/projects-front/-/tree/release_v0.13.1)

### Frontend - Home

\#\#\# run FRONT

1.  Go to \`/WWW/FRONT\`

2.  Run \`npm run dev\` your web application will be available on
    \`*https://dev.cri-paris.org:\<\<port\#\>\>*\` Change with the right
    port of your env !

3.  Constants are in \`dist/const.js\` Some are set up within the env
    creation. For more details go \[here\](front/constants.md)

### Backend - Home

\#\#\# run BACK

1.  The backend is already running!

2.  If something went wrong and you need to re-launch the back process:
    '*sudo touch /etc/uwsgi-emperor/vassals/apiprojectsdev.ini*'. This
    command needs to be run after any modification of 'settings.py'.

3.  Access logs: '*sudo tail -f
    /var/log/uwsgi/vassals/apiprojectsdev.log*'.

4.  Constants are in '*/const.py*' Some are set up within the env
    creation. For more details go '*back/constants.md*'.

### Database

\#\#\# run MONGO

MongoDB CRUD operations create, read, update, and delete dB documents:

1.  To access Mongo CRUD operations, modify dB.

2.  Just run \`mongo\`.

3.  Choose the right DB (default: '*apiprojectsdev*') using 'use'.

4.  Start querying using common commands
    [[here]{.ul}](https://docs.mongodb.com/manual/reference/mongo-shell/)

#### Create Operations

Create or insert operations add new
[documents](https://docs.mongodb.com/manual/core/document/#bson-document-format)
to a
[collection](https://docs.mongodb.com/manual/core/databases-and-collections/#collections).
If the collection does not currently exist, insert operations will
create the collection.

MongoDB provides the following methods to insert documents into a
collection:

-   [db.collection.insertOne()](https://docs.mongodb.com/manual/reference/method/db.collection.insertOne/#db.collection.insertOne)
    *New in version 3.2*

-   [db.collection.insertMany()](https://docs.mongodb.com/manual/reference/method/db.collection.insertMany/#db.collection.insertMany)
    *New in version 3.2*

In MongoDB, insert operations target a single
[collection](https://docs.mongodb.com/manual/reference/glossary/#term-collection).
All write operations in MongoDB are
[atomic](https://docs.mongodb.com/manual/core/write-operations-atomicity/)
on the level of a single
[document](https://docs.mongodb.com/manual/core/document/).

For examples, see [Insert
Documents](https://docs.mongodb.com/manual/tutorial/insert-documents/).

#### Read Operations

Read operations retrieve
[documents](https://docs.mongodb.com/manual/core/document/#bson-document-format)
from a
[collection](https://docs.mongodb.com/manual/core/databases-and-collections/#collections);
i.e. query a collection for documents. MongoDB provides the following
methods to read documents from a collection:

-   [db.collection.find()](https://docs.mongodb.com/manual/reference/method/db.collection.find/#db.collection.find)

You can specify [query filters or
criteria](https://docs.mongodb.com/manual/tutorial/query-documents/#read-operations-query-argument)
that identify the documents to return.

For examples, see:

-   [Query
    Documents](https://docs.mongodb.com/manual/tutorial/query-documents/)

-   [Query on Embedded/Nested
    Documents](https://docs.mongodb.com/manual/tutorial/query-embedded-documents/)

-   [Query an
    Array](https://docs.mongodb.com/manual/tutorial/query-arrays/)

-   [Query an Array of Embedded
    Documents](https://docs.mongodb.com/manual/tutorial/query-array-of-documents/)

#### Update Operations

Update operations modify existing
[documents](https://docs.mongodb.com/manual/core/document/#bson-document-format)
in a
[collection](https://docs.mongodb.com/manual/core/databases-and-collections/#collections).
MongoDB provides the following methods to update documents of a
collection:

-   [db.collection.updateOne()](https://docs.mongodb.com/manual/reference/method/db.collection.updateOne/#db.collection.updateOne)
    *New in version 3.2*

-   [db.collection.updateMany()](https://docs.mongodb.com/manual/reference/method/db.collection.updateMany/#db.collection.updateMany)
    *New in version 3.2*

-   [db.collection.replaceOne()](https://docs.mongodb.com/manual/reference/method/db.collection.replaceOne/#db.collection.replaceOne)
    *New in version 3.2*

In MongoDB, update operations target a single collection. All write
operations in MongoDB are
[atomic](https://docs.mongodb.com/manual/core/write-operations-atomicity/)
on the level of a single document.

You can specify criteria, or filters, that identify the documents to
update. These
[filters](https://docs.mongodb.com/manual/core/document/#document-query-filter)
use the same syntax as read operations.

For examples, see [Update
Documents](https://docs.mongodb.com/manual/tutorial/update-documents/).

#### Delete Operations

Delete operations remove documents from a collection. MongoDB provides
the following methods to delete documents of a collection:

-   [db.collection.deleteOne()](https://docs.mongodb.com/manual/reference/method/db.collection.deleteOne/#db.collection.deleteOne)
    *New in version 3.2*

-   [db.collection.deleteMany()](https://docs.mongodb.com/manual/reference/method/db.collection.deleteMany/#db.collection.deleteMany)
    *New in version 3.2*

In MongoDB, delete operations target a single
[collection](https://docs.mongodb.com/manual/reference/glossary/#term-collection).
All write operations in MongoDB are
[atomic](https://docs.mongodb.com/manual/core/write-operations-atomicity/)
on the level of a single document.

You can specify criteria, or filters, that identify the documents to
remove. These
[filters](https://docs.mongodb.com/manual/core/document/#document-query-filter)
use the same syntax as read operations.

For examples, see [Delete
Documents](https://docs.mongodb.com/manual/tutorial/remove-documents/).

#### Bulk Write

MongoDB provides the ability to perform write operations in bulk. For
details, see [Bulk Write
Operations](https://docs.mongodb.com/manual/core/bulk-write-operations/).

### Versioning

\#\#\# GIT

Here you can access the complete documentation for GitLab, the single
application for the [entire DevOps
lifecycle](https://docs.gitlab.com/ee/README.html#the-entire-devops-lifecycle).

#### Key relevant GitLab documentation

+----------------------------------+----------------------------------+
| **Essential documentation**      | **Essential documentation**      |
+==================================+==================================+
| [User                            | [Administrator                   |
| documentation](https://doc       | docu                             |
| s.gitlab.com/ee/user/index.html) | mentation](https://docs.gitlab.c |
|                                  | om/ee/administration/index.html) |
| Discover features and concepts   |                                  |
| for GitLab users.                | Everything GitLab self-managed   |
|                                  | administrators need to know.     |
+----------------------------------+----------------------------------+
| [Contributing to                 | [New to Git and                  |
| GitLab                           | GitLab                           |
| ](https://docs.gitlab.com/ee/REA | ?](https://docs.gitlab.com/ee/RE |
| DME.html#contributing-to-gitlab) | ADME.html#new-to-git-and-gitlab) |
|                                  |                                  |
| At GitLab, everyone can          | We have the resources to get you |
| contribute!                      | started.                         |
+----------------------------------+----------------------------------+
| [Build an integration with       | [Coming to GitLab from another   |
| GitLab](https://                 | platform?](https://docs.g        |
| docs.gitlab.com/ee/README.html#b | itlab.com/ee/README.html#coming- |
| uild-an-integration-with-gitlab) | to-gitlab-from-another-platform) |
|                                  |                                  |
| Consult our integration          | Consult our guides.              |
| documentation.                   |                                  |
+----------------------------------+----------------------------------+
| [Install                         | [Customers](https://docs.gitlab. |
| GitLab](ht                       | com/ee/subscriptions/index.html) |
| tps://about.gitlab.com/install/) |                                  |
|                                  | Information for new and existing |
| Installation options for         | customers.                       |
| different platforms.             |                                  |
+----------------------------------+----------------------------------+
| [Update                          | [Reference                       |
| GitLab](https://docs.            | Architectures](https://docs.     |
| gitlab.com/ee/update/index.html) | gitlab.com/ee/administration/ref |
|                                  | erence_architectures/index.html) |
| Update your GitLab self-managed  |                                  |
| instance to the latest version.  | GitLab reference architectures.  |
+----------------------------------+----------------------------------+
| [GitLab                          |                                  |
| releases](htt                    |                                  |
| ps://about.gitlab.com/releases/) |                                  |
|                                  |                                  |
| What's new in GitLab.            |                                  |
+----------------------------------+----------------------------------+

#### Popular topics

Have a look at some of our most popular topics:

  **Popular topic**                                                                                             **Description**
  ------------------------------------------------------------------------------------------------------------- ----------------------------------------------------------------------------
  [Two-factor authentication](https://docs.gitlab.com/ee/user/profile/account/two_factor_authentication.html)   Improve the security of your GitLab account.
  [GitLab groups](https://docs.gitlab.com/ee/user/group/index.html)                                             Manage projects together.
  [GitLab CI/CD pipeline configuration reference](https://docs.gitlab.com/ee/ci/yaml/README.html)               Available configuration options for .gitlab-ci.yml files.
  [Activate GitLab EE with a license](https://docs.gitlab.com/ee/user/admin_area/license.html)                  Activate GitLab Enterprise Edition functionality with a license.
  [Back up and restore GitLab](https://docs.gitlab.com/ee/raketasks/backup_restore.html)                        Rake tasks for backing up and restoring GitLab self-managed instances.
  [GitLab release and maintenance policy](https://docs.gitlab.com/ee/policy/maintenance.html)                   Policies for version naming and cadence, and also upgrade recommendations.
  [Elasticsearch integration](https://docs.gitlab.com/ee/integration/elasticsearch.html)                        Integrate Elasticsearch with GitLab to enable advanced searching.
  [Omnibus GitLab database settings](https://docs.gitlab.com/omnibus/settings/database.html)                    Database settings for Omnibus GitLab self-managed instances.
  [Omnibus GitLab NGINX settings](https://docs.gitlab.com/omnibus/settings/nginx.html)                          NGINX settings for Omnibus GitLab self-managed instances.
  [Omnibus GitLab SSL configuration](https://docs.gitlab.com/omnibus/settings/ssl.html)                         SSL settings for Omnibus GitLab self-managed instances.
  [GitLab.com settings](https://docs.gitlab.com/ee/user/gitlab_com/index.html)                                  Settings used for GitLab.com.

#### The entire DevOps lifecycle

GitLab is the application for software development, security, and
operations that enables [Concurrent
DevOps](https://about.gitlab.com/topics/concurrent-devops/). GitLab
makes the software lifecycle faster and radically improves the speed of
business. Git is directly configured so you can add your own gitlab CRI
alias and start creating your own feature branch.

# Introduction

Projects platform to reference a community\'s projects and is home to a
community of passionate, inspiring projects that are launched there
every day.

Nevertheless, it is difficult to know what is going on there every day,
and we all \"miss\" many daily achievements. Because of a lack of
visibility, some projects lose the opportunity for better support, and
precious resources are spent on redundant ideas.

### Helping the community

We believe that it will also make it easier to train teams on certain
subjects by allowing them to better identify the skills and achievements
already available or in gestation.

It is also a way to get to know the people in the community or who
revolve around the organization and its projects, in line with the
objectives of sustainable development defined by the United Nations.

### Communicate better

This platform will enhance the organization\'s impact by simply
presenting the extent of its creative force and potential.

This will benefit everyone, with each project benefiting from
centralized and broader communication.

Indeed Projects Platform is, as well as CRI people, a data source for
all CRI\'s digital means of communication, avoiding - badly - duplicated
information.

### What fields are included in a project?

When you create a new project, you create a title, an image,
contributors and you can annotate it by UNESCO\'s sustainable
development objectives to which it is addressed and by keywords. These
keywords are chosen from all available Wikipedia article titles. They
make it easy to find projects with similarities. In the following, they
will also be visualized and shared on the WeLearn cartography.

## What is a Projects Platform?

In order to better share ideas worth sharing with everyone, we have
created the Projects platform for presentation and referencing of all
projects that are intended to be collaborative and easy to access, it
will allow everyone to have a directory of the many projects carried out
and to present their own achievements.

We also believe that other organizations have the same need for better
project sharing. We propose that they benefit from this tool.

### Getting Started

#### Our current Projects platform folder structure

#### **Key Folders**

##### Application Dialogs (appdialogs)

Pop-in component for Description and Blog. Vue component inside should
be moved in shrcomponents or wins

##### Assets (assets)

Fonts and global images. Warning : Images are now in a file system based
so no new images should be added here and the /img subfolder might be
deleted.

##### Global Functions (functs)

Global function that can be reused. It should contain services. Some
functions might be added in a mixin.

##### Mixins (mixins) 

Component function that can be added in more than one component. Refers
to vue documentation to understand the meaning of a mixin.

##### Mini Pop-in Windows(miniwins)

Small pop-in component. It would be better to have few functional pop-in
component and inject only text in it.

##### Pages (pages)

It should only contain user pages and those pages components should be
built with other component.

##### Popups (popups)

Popup components

##### SCSS (scss)

SCSS global files

##### Shared Components (shrcomponents)

All reusable components. All components expect pages and one used
component should be here. Even wins and miniwins.

##### Windows (wins)

Large pop-in components

#### **Custom Vue Event Bus (VBUS)**

To understand VBUS is critical to understand Projects Platform component
event communication. We currently don't use Vuex that could be a better
way to manage state and data flow across components. We are utilizing
VBUS currently to connect unrelated sections of our VueJs
Application/Codebase talk to each other with current project code event
bus/publisher-subscriber pattern. The same has provided flexibility to
have communication between unrelated or sibling relationships but can
very easily create ambiguous and unmanageable state management within an
application as complex as the Projects Platform. So the next stage of
optimization of Projects would include re-architecting the application
and include Vuex to alter a global state that all components check for
via getters instead of VBUS.

So then in a completely unrelated component you would need to hook into
that event and react to it, I find myself registering the event hooks in
the components mounted() lifecycle hook to be able to listen to events.
Similar to child to parent communication but the difference is the
component reacting to the event registers its listener in a different
place (in this case in the mounted hook). Now you have the ability for
one component to speak to another component in a different part of your
application. It is a handy thing to know but of course beware of
overusing this. It could get mucky or used where a different approach
might better suit. So these event systems come part and parcel of Vue
and can be utilised to achieve component communication in a variety of
ways.

The Publisher-Subscriber pattern we will use to allow components to
subscribe to an event. Then other components can publish an event and
all subscribers can then react to that. Two main methods to allow
subscription and the ability to publish to those subscribers. Again this
then means we get access in every component to the PubSub instance via
this.\$pubSub. So then we must subscribe to some components, a good
example would be a bunch of show/hide panel components, they all can
open independently. You wish to have a button elsewhere in the
application that you would want to have the ability to close all those
other panel components with one click. So here we see that we will use
mounted() to subscribe to an event called closePanels. When it is
invoked then we will run our localMethod to close the panel. So this
time our click event will run this. \$pubSub.publish('closePanels'),
which will inform all subscribers to run and thus close them all. We
have run through different ways to utilise communication throughout your
VueJs Application. We have used event systems and we have used some
patterns to help the way these components communicate. Again it is
trying to find the right time to use each and when.

# Application & Component Instances

## Creating an Application Instance

Every Vue application starts by creating a new application instance with
the createApp function:

const app = Vue.createApp({

/\* options \*/

})

The application instance is used to register \'globals\' that can then
be used by components within that application. We\'ll discuss that in
detail later in the guide but as a quick example:

const app = Vue.createApp({})

app.component(\'SearchInput\', SearchInputComponent)

app.directive(\'focus\', FocusDirective)

app.use(LocalePlugin)

Most of the methods exposed by the application instance return that same
instance, allowing for chaining:

Vue.createApp({})

.component(\'SearchInput\', SearchInputComponent)

.directive(\'focus\', FocusDirective)

.use(LocalePlugin)

You can browse the full application API in the [[API
reference]{.ul}](https://v3.vuejs.org/api/application-api.html).

## [\#](https://v3.vuejs.org/guide/instance.html#the-root-component)The Root Component

The options passed to createApp are used to configure the root
component. That component is used as the starting point for rendering
when we mount the application.

An application needs to be mounted into a DOM element. For example, if
we want to mount a Vue application into \<div id=\"app\"\>\</div\>, we
should pass \#app:

const RootComponent = {

/\* options \*/

}

const app = Vue.createApp(RootComponent)

const vm = app.mount(\'\#app\')

Unlike most of the application methods, mount does not return the
application. Instead it returns the root component instance.

Although not strictly associated with the [[MVVM
pattern]{.ul}](https://en.wikipedia.org/wiki/Model_View_ViewModel),
Vue\'s design was partly inspired by it. As a convention, we often use
the variable vm (short for ViewModel) to refer to a component instance.

While all the examples on this page only need a single component, most
real applications are organized into a tree of nested, reusable
components. For example, a Todo application\'s component tree might look
like this:

Root Component

└─ TodoList

├─ TodoItem

│ ├─ DeleteTodoButton

│ └─ EditTodoButton

└─ TodoListFooter

├─ ClearTodosButton

└─ TodoListStatistics

Each component will have its own component instance, vm. For some
components, such as TodoItem, there will likely be multiple instances
rendered at any one time. All of the component instances in this
application will share the same application instance.

We\'ll talk about [the component
system](https://v3.vuejs.org/guide/component-basics.html) in detail
later. For now, just be aware that the root component isn\'t really any
different from any other component. The configuration options are the
same, as is the behavior of the corresponding component instance.

## [\#](https://v3.vuejs.org/guide/instance.html#component-instance-properties)Component Instance Properties

Earlier in the guide we met data properties. Properties defined in data
are exposed via the component instance:

const app = Vue.createApp({

data() {

return { count: 4 }

}

})

const vm = app.mount(\'\#app\')

console.log(vm.count) // =\> 4

There are various other component options that add user-defined
properties to the component instance, such as methods, props, computed,
inject and setup. We\'ll discuss each of these in depth later in the
guide. All of the properties of the component instance, no matter how
they are defined, will be accessible in the component\'s template.

Vue also exposes some built-in properties via the component instance,
such as \$attrs and \$emit. These properties all have a \$ prefix to
avoid conflicting with user-defined property names.

## [\#](https://v3.vuejs.org/guide/instance.html#lifecycle-hooks)Lifecycle Hooks

Each component instance goes through a series of initialization steps
when it\'s created - for example, it needs to set up data observation,
compile the template, mount the instance to the DOM, and update the DOM
when data changes. Along the way, it also runs functions called
lifecycle hooks, giving users the opportunity to add their own code at
specific stages.

For example, the
[created](https://v3.vuejs.org/api/options-lifecycle-hooks.html#created)
hook can be used to run code after an instance is created:

Vue.createApp({

data() {

return { count: 1 }

},

created() {

// \`this\` points to the vm instance

console.log(\'count is: \' + this.count) // =\> \"count is: 1\"

}

})

There are also other hooks which will be called at different stages of
the instance\'s lifecycle, such as
[mounted](https://v3.vuejs.org/api/options-lifecycle-hooks.html#mounted),
[updated](https://v3.vuejs.org/api/options-lifecycle-hooks.html#updated),
and
[unmounted](https://v3.vuejs.org/api/options-lifecycle-hooks.html#unmounted).
All lifecycle hooks are called with this context pointing to the current
active instance invoking it

Don\'t use [arrow
functions](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Functions/Arrow_functions)
on an options property or callback, such as created: () =\>
console.log(this.a) or vm.\$watch(\'a\', newValue =\> this.myMethod()).
Since an arrow function doesn\'t have a this, this will be treated as
any other variable and lexically looked up through parent scopes until
found, often resulting in errors such as Uncaught TypeError: Cannot read
property of undefined or Uncaught TypeError: this.myMethod is not a
function.

## [\#](https://v3.vuejs.org/guide/instance.html#lifecycle-diagram)Lifecycle Diagram

Below is a diagram for the instance lifecycle. You don\'t need to fully
understand everything going on right now, but as you learn and build
more, it will be a useful
reference.![](media/image1.png){width="4.65625in"
height="7.683337707786527in"}

# Template Syntax

Vue.js uses an HTML-based template syntax that allows you to
declaratively bind the rendered DOM to the underlying component
instance\'s data. All Vue.js templates are valid HTML that can be parsed
by spec-compliant browsers and HTML parsers.

Under the hood, Vue compiles the templates into Virtual DOM render
functions. Combined with the reactivity system, Vue is able to
intelligently figure out the minimal number of components to re-render
and apply the minimal amount of DOM manipulations when the app state
changes.

If you are familiar with Virtual DOM concepts and prefer the raw power
of JavaScript, you can also [[directly write render
functions]{.ul}](https://v3.vuejs.org/guide/render-function.html)
instead of templates, with optional JSX support.

## [\#](https://v3.vuejs.org/guide/template-syntax.html#interpolations)Interpolations

### [\#](https://v3.vuejs.org/guide/template-syntax.html#text)Text

The most basic form of data binding is text interpolation using the
\"Mustache\" syntax (double curly braces):

\<span\>Message: {{ msg }}\</span\>

The mustache tag will be replaced with the value of the msg property
from the corresponding component instance. It will also be updated
whenever the msg property changes.

You can also perform one-time interpolations that do not update on data
change by using the [[v-once
directive]{.ul}](https://v3.vuejs.org/api/directives.html#v-once), but
keep in mind this will also affect any other bindings on the same node:

\<span v-once\>This will never change: {{ msg }}\</span\>

### [\#](https://v3.vuejs.org/guide/template-syntax.html#raw-html)Raw HTML

The double mustaches interpret the data as plain text, not HTML. In
order to output real HTML, you will need to use the [[v-html]{.ul}
[directive]{.ul}](https://v3.vuejs.org/api/directives.html#v-html):

\<p\>Using mustaches: {{ rawHtml }}\</p\>

\<p\>Using v-html directive: \<span v-html=\"rawHtml\"\>\</span\>\</p\>

The contents of the span will be replaced with the value of the rawHtml
property, interpreted as plain HTML - data bindings are ignored. Note
that you cannot use v-html to compose template partials, because Vue is
not a string-based templating engine. Instead, components are preferred
as the fundamental unit for UI reuse and composition.

TIP

Dynamically rendering arbitrary HTML on your website can be very
dangerous because it can easily lead to XSS vulnerabilities

. Only use HTML interpolation on trusted content and never on
user-provided content

### [\#](https://v3.vuejs.org/guide/template-syntax.html#attributes)Attributes

Mustaches cannot be used inside HTML attributes. Instead, use a
[[v-bind]{.ul}
[directive]{.ul}](https://v3.vuejs.org/api/directives.html#v-bind):

\<div v-bind:id=\"dynamicId\"\>\</div\>

If the bound value is null or undefined then the attribute will not be
included on the rendered element.

In the case of boolean attributes, where their mere existence implies
true, v-bind works a little differently. For example:

\<button v-bind:disabled=\"isButtonDisabled\"\>Button\</button\>

The disabled attribute will be included if isButtonDisabled has a truthy
value. It will also be included if the value is an empty string,
maintaining consistency with \<button disabled=\"\"\>. For other falsy
values the attribute will be omitted.

### [\#](https://v3.vuejs.org/guide/template-syntax.html#using-javascript-expressions)Using JavaScript Expressions

So far we\'ve only been binding to simple property keys in our
templates. But Vue.js actually supports the full power of JavaScript
expressions inside all data bindings:

{{ number + 1 }}

{{ ok ? \'YES\' : \'NO\' }}

{{ message.split(\'\').reverse().join(\'\') }}

\<div v-bind:id=\"\'list-\' + id\"\>\</div\>

These expressions will be evaluated as JavaScript in the data scope of
the current active instance. One restriction is that each binding can
only contain one single expression, so the following will NOT work:

\<!\-- this is a statement, not an expression: \--\>

{{ var a = 1 }}

\<!\-- flow control won\'t work either, use ternary expressions \--\>

{{ if (ok) { return message } }}

## [\#](https://v3.vuejs.org/guide/template-syntax.html#directives)Directives

Directives are special attributes with the v- prefix. Directive
attribute values are expected to be a single JavaScript expression (with
the exception of v-for and v-on, which will be discussed later). A
directive\'s job is to reactively apply side effects to the DOM when the
value of its expression changes. Let\'s review the example we saw in the
introduction:

\<p v-if=\"seen\"\>Now you see me\</p\>

Here, the v-if directive would remove/insert the \<p\> element based on
the truthiness of the value of the expression seen.

### [\#](https://v3.vuejs.org/guide/template-syntax.html#arguments)Arguments

Some directives can take an \"argument\", denoted by a colon after the
directive name. For example, the v-bind directive is used to reactively
update an HTML attribute:

\<a v-bind:href=\"url\"\> \... \</a\>

Here href is the argument, which tells the v-bind directive to bind the
element\'s href attribute to the value of the expression url.

Another example is the v-on directive, which listens to DOM events:

\<a v-on:click=\"doSomething\"\> \... \</a\>

Here the argument is the event name to listen to. We will talk about
event handling in more detail too.

### [\#](https://v3.vuejs.org/guide/template-syntax.html#dynamic-arguments)Dynamic Arguments

It is also possible to use a JavaScript expression in a directive
argument by wrapping it with square brackets:

\<!\--

Note that there are some constraints to the argument expression, as
explained

in the \"Dynamic Argument Expression Constraints\" section below.

\--\>

\<a v-bind:\[attributeName\]=\"url\"\> \... \</a\>

Here attributeName will be dynamically evaluated as a JavaScript
expression, and its evaluated value will be used as the final value for
the argument. For example, if your component instance has a data
property, attributeName, whose value is \"href\", then this binding will
be equivalent to v-bind:href.

Similarly, you can use dynamic arguments to bind a handler to a dynamic
event name:

\<a v-on:\[eventName\]=\"doSomething\"\> \... \</a\>

In this example, when eventName\'s value is \"focus\",
v-on:\[eventName\] will be equivalent to v-on:focus.

### [\#](https://v3.vuejs.org/guide/template-syntax.html#modifiers)Modifiers

Modifiers are special postfixes denoted by a dot, which indicate that a
directive should be bound in some special way. For example, the .prevent
modifier tells the v-on directive to call event.preventDefault() on the
triggered event:

\<form v-on:submit.prevent=\"onSubmit\"\>\...\</form\>

You\'ll see other examples of modifiers later, [[for]{.ul}
[v-on]{.ul}](https://v3.vuejs.org/guide/events.html#event-modifiers) and
[[for]{.ul}
[v-model]{.ul}](https://v3.vuejs.org/guide/forms.html#modifiers), when
we explore those features.

## [\#](https://v3.vuejs.org/guide/template-syntax.html#shorthands)Shorthands

The v- prefix serves as a visual cue for identifying Vue-specific
attributes in your templates. This is useful when you are using Vue.js
to apply dynamic behavior to some existing markup, but can feel verbose
for some frequently used directives. At the same time, the need for the
v- prefix becomes less important when you are building a
[[SPA]{.ul}](https://en.wikipedia.org/wiki/Single-page_application),
where Vue manages every template. Therefore, Vue provides special
shorthands for two of the most often used directives, v-bind and v-on:

[[\#]{.ul}](https://v3.vuejs.org/guide/template-syntax.html#v-bind-shorthand)v-bind

\<!\-- full syntax \--\>

\<a v-bind:href=\"url\"\> \... \</a\>

\<!\-- shorthand \--\>

\<a :href=\"url\"\> \... \</a\>

\<!\-- shorthand with dynamic argument \--\>

\<a :\[key\]=\"url\"\> \... \</a\>

[[\#]{.ul}](https://v3.vuejs.org/guide/template-syntax.html#v-on-shorthand)v-on
Shorthand

\<!\-- full syntax \--\>

\<a v-on:click=\"doSomething\"\> \... \</a\>

\<!\-- shorthand \--\>

\<a \@click=\"doSomething\"\> \... \</a\>

\<!\-- shorthand with dynamic argument \--\>

\<a @\[event\]=\"doSomething\"\> \... \</a\>

They may look a bit different from normal HTML, but : and @ are valid
characters for attribute names and all Vue-supported browsers can parse
it correctly. In addition, they do not appear in the final rendered
markup. The shorthand syntax is totally optional, but you will likely
appreciate it when you learn more about its usage later.

### [\#](https://v3.vuejs.org/guide/template-syntax.html#caveats)Caveats

#### [\#](https://v3.vuejs.org/guide/template-syntax.html#dynamic-argument-value-constraints)Dynamic Argument Value Constraints

Dynamic arguments are expected to evaluate to a string, with the
exception of null. The special value null can be used to explicitly
remove the binding. Any other non-string value will trigger a warning.

#### [\#](https://v3.vuejs.org/guide/template-syntax.html#dynamic-argument-expression-constraints)Dynamic Argument Expression Constraints

Dynamic argument expressions have some syntax constraints because
certain characters, such as spaces and quotes, are invalid inside HTML
attribute names. For example, the following is invalid:

\<!\-- This will trigger a compiler warning. \--\>

\<a v-bind:\[\'foo\' + bar\]=\"value\"\> \... \</a\>

We recommend replacing any complex expressions with a [[computed
property]{.ul}](https://v3.vuejs.org/guide/computed.html), one of the
most fundamental pieces of Vue, which we\'ll cover shortly.

When using in-DOM templates (templates directly written in an HTML
file), you should also avoid naming keys with uppercase characters, as
browsers will coerce attribute names into lowercase:

\<!\--

This will be converted to v-bind:\[someattr\] in in-DOM templates.

Unless you have a \"someattr\" property in your instance, your code
won\'t work.

\--\>

\<a v-bind:\[someAttr\]=\"value\"\> \... \</a\>

Template expressions are sandboxed and only have access to a [whitelist
of globals]{.ul}

such as Math and Date. You should not attempt to access user defined
globals in template expressions.

# Data Properties and Methods

## [\#](https://v3.vuejs.org/guide/data-methods.html#data-properties)Data Properties

The data option for a component is a function. Vue calls this function
as part of creating a new component instance. It should return an
object, which Vue will then wrap in its reactivity system and store on
the component instance as \$data. For convenience, any top-level
properties of that object are also exposed directly via the component
instance:

const app = Vue.createApp({

data() {

return { count: 4 }

}

})

const vm = app.mount(\'\#app\')

console.log(vm.\$data.count) // =\> 4

console.log(vm.count) // =\> 4

// Assigning a value to vm.count will also update \$data.count

vm.count = 5

console.log(vm.\$data.count) // =\> 5

// \... and vice-versa

vm.\$data.count = 6

console.log(vm.count) // =\> 6

These instance properties are only added when the instance is first
created, so you need to ensure they are all present in the object
returned by the data function. Where necessary, use null, undefined or
some other placeholder value for properties where the desired value
isn\'t yet available.

It is possible to add a new property directly to the component instance
without including it in data. However, because this property isn\'t
backed by the reactive \$data object, it won\'t automatically be tracked
by [[Vue\'s reactivity
system]{.ul}](https://v3.vuejs.org/guide/reactivity.html).

Vue uses a \$ prefix when exposing its own built-in APIs via the
component instance. It also reserves the prefix \_ for internal
properties. You should avoid using names for top-level data properties
that start with either of these characters.

## [\#](https://v3.vuejs.org/guide/data-methods.html#methods)Methods

To add methods to a component instance we use the methods option. This
should be an object containing the desired methods:

const app = Vue.createApp({

data() {

return { count: 4 }

},

methods: {

increment() {

// \`this\` will refer to the component instance

this.count++

}

}

})

const vm = app.mount(\'\#app\')

console.log(vm.count) // =\> 4

vm.increment()

console.log(vm.count) // =\> 5

Vue automatically binds the this value for methods so that it always
refers to the component instance. This ensures that a method retains the
correct this value if it\'s used as an event listener or callback. You
should avoid using arrow functions when defining methods, as that
prevents Vue from binding the appropriate this value.

Just like all other properties of the component instance, the methods
are accessible from within the component\'s template. Inside a template
they are most commonly used as event listeners:

\<button \@click=\"increment\"\>Up vote\</button\>

In the example above, the method increment will be called when the
\<button\> is clicked.

It is also possible to call a method directly from a template. As we\'ll
see shortly, it\'s usually better to use a [[computed
property]{.ul}](https://v3.vuejs.org/guide/computed.html) instead.
However, using a method can be useful in scenarios where computed
properties aren\'t a viable option. You can call a method anywhere that
a template supports JavaScript expressions:

\<span :title=\"toTitleDate(date)\"\>

{{ formatDate(date) }}

\</span\>

If the methods toTitleDate or formatDate access any reactive data then
it will be tracked as a rendering dependency, just as if it had been
used in the template directly.

Methods called from a template should not have any side effects, such as
changing data or triggering asynchronous processes. If you find yourself
tempted to do that you should probably use a [[lifecycle
hook]{.ul}](https://v3.vuejs.org/guide/instance.html#lifecycle-hooks)
instead.

[[\#]{.ul}](https://v3.vuejs.org/guide/data-methods.html#debouncing-and-throttling)Debouncing
and Throttling

Vue doesn\'t include built-in support for debouncing or throttling but
it can be implemented using libraries such as
[[Lodash]{.ul}](https://lodash.com/).

In cases where a component is only used once, the debouncing can be
applied directly within methods:

\<script
src=\"https://unpkg.com/lodash\@4.17.20/lodash.min.js\"\>\</script\>

\<script\>

Vue.createApp({

methods: {

// Debouncing with Lodash

click: \_.debounce(function() {

// \... respond to click \...

}, 500)

}

}).mount(\'\#app\')

\</script\>

However, this approach is potentially problematic for components that
are reused because they\'ll all share the same debounced function. To
keep the component instances independent from each other, we can add the
debounced function in the created lifecycle hook:

app.component(\'save-button\', {

created() {

// Debouncing with Lodash

this.debouncedClick = \_.debounce(this.click, 500)

},

unmounted() {

// Cancel the timer when the component is removed

this.debouncedClick.cancel()

},

methods: {

click() {

// \... respond to click \...

}

},

template: \`

\<button \@click=\"debouncedClick\"\>

Save

\</button\>

\`

})

# Computed Properties and Watchers

## [\#](https://v3.vuejs.org/guide/computed.html#computed-properties)Computed Properties

In-template expressions are very convenient, but they are meant for
simple operations. Putting too much logic in your templates can make
them bloated and hard to maintain. For example, if we have an object
with a nested array:

Vue.createApp({

data() {

return {

author: {

name: \'John Doe\',

books: \[

\'Vue 2 - Advanced Guide\',

\'Vue 3 - Basic Guide\',

\'Vue 4 - The Mystery\'

\]

}

}

}

})

And we want to display different messages depending on if author already
has some books or not

\<div id=\"computed-basics\"\>

\<p\>Has published books:\</p\>

\<span\>{{ author.books.length \> 0 ? \'Yes\' : \'No\' }}\</span\>

\</div\>

At this point, the template is no longer simple and declarative. You
have to look at it for a second before realizing that it performs a
calculation depending on author.books. The problem is made worse when
you want to include this calculation in your template more than once.

That\'s why for complex logic that includes reactive data, you should
use a computed property.

### [\#](https://v3.vuejs.org/guide/computed.html#basic-example)Basic Example

\<div id=\"computed-basics\"\>

\<p\>Has published books:\</p\>

\<span\>{{ publishedBooksMessage }}\</span\>

\</div\>

Vue.createApp({

data() {

return {

author: {

name: \'John Doe\',

books: \[

\'Vue 2 - Advanced Guide\',

\'Vue 3 - Basic Guide\',

\'Vue 4 - The Mystery\'

\]

}

}

},

computed: {

// a computed getter

publishedBooksMessage() {

// \`this\` points to the vm instance

return this.author.books.length \> 0 ? \'Yes\' : \'No\'

}

}

}).mount(\'\#computed-basics\')

Result:

Here we have declared a computed property publishedBooksMessage.

Try to change the value of books array in the application data and you
will see how publishedBooksMessage is changing accordingly.

You can data-bind to computed properties in templates just like a normal
property. Vue is aware that vm.publishedBooksMessage depends on
vm.author.books, so it will update any bindings that depend on
vm.publishedBooksMessage when vm.author.books changes. And the best part
is that we\'ve created this dependency relationship declaratively: the
computed getter function has no side effects, which makes it easier to
test and understand.

### [\#](https://v3.vuejs.org/guide/computed.html#computed-caching-vs-methods)Computed Caching vs Methods

You may have noticed we can achieve the same result by invoking a method
in the expression:

\<p\>{{ calculateBooksMessage() }}\</p\>

// in component

methods: {

calculateBooksMessage() {

return this.author.books.length \> 0 ? \'Yes\' : \'No\'

}

}

Instead of a computed property, we can define the same function as a
method. For the end result, the two approaches are indeed exactly the
same. However, the difference is that computed properties are cached
based on their reactive dependencies. A computed property will only
re-evaluate when some of its reactive dependencies have changed. This
means as long as author.books has not changed, multiple access to the
publishedBooksMessage computed property will immediately return the
previously computed result without having to run the function again.

This also means the following computed property will never update,
because Date.now() is not a reactive dependency:

computed: {

now() {

return Date.now()

}

}

In comparison, a method invocation will always run the function whenever
a re-render happens.

Why do we need caching? Imagine we have an expensive computed property
list, which requires looping through a huge array and doing a lot of
computations. Then we may have other computed properties that in turn
depend on list. Without caching, we would be executing list's getter
many more times than necessary! In cases where you do not want caching,
use a method instead.

### [\#](https://v3.vuejs.org/guide/computed.html#computed-setter)Computed Setter

Computed properties are by default getter-only, but you can also provide
a setter when you need it:

// \...

computed: {

fullName: {

// getter

get() {

return this.firstName + \' \' + this.lastName

},

// setter

set(newValue) {

const names = newValue.split(\' \')

this.firstName = names\[0\]

this.lastName = names\[names.length - 1\]

}

}

}

// \...

Now when you run vm.fullName = \'John Doe\', the setter will be invoked
and vm.firstName and vm.lastName will be updated accordingly.

## [\#](https://v3.vuejs.org/guide/computed.html#watchers)Watchers

While computed properties are more appropriate in most cases, there are
times when a custom watcher is necessary. That\'s why Vue provides a
more generic way to react to data changes through the watch option. This
is most useful when you want to perform asynchronous or expensive
operations in response to changing data.

For example:

\<div id=\"watch-example\"\>

\<p\>

Ask a yes/no question:

\<input v-model=\"question\" /\>

\</p\>

\<p\>{{ answer }}\</p\>

\</div\>

\<!\-- Since there is already a rich ecosystem of ajax libraries \--\>

\<!\-- and collections of general-purpose utility methods, Vue core
\--\>

\<!\-- is able to remain small by not reinventing them. This also \--\>

\<!\-- gives you the freedom to use what you\'re familiar with. \--\>

\<script
src=\"https://cdn.jsdelivr.net/npm/axios\@0.12.0/dist/axios.min.js\"\>\</script\>

\<script\>

const watchExampleVM = Vue.createApp({

data() {

return {

question: \'\',

answer: \'Questions usually contain a question mark. ;-)\'

}

},

watch: {

// whenever question changes, this function will run

question(newQuestion, oldQuestion) {

if (newQuestion.indexOf(\'?\') \> -1) {

this.getAnswer()

}

}

},

methods: {

getAnswer() {

this.answer = \'Thinking\...\'

axios

.get(\'https://yesno.wtf/api\')

.then(response =\> {

this.answer = response.data.answer

})

.catch(error =\> {

this.answer = \'Error! Could not reach the API. \' + error

})

}

}

}).mount(\'\#watch-example\')

\</script\>

Result:

In this case, using the watch option allows us to perform an
asynchronous operation (accessing an API) and sets a condition for
performing this operation. None of that would be possible with a
computed property.

In addition to the watch option, you can also use the imperative
[vm.\$watch API](https://v3.vuejs.org/api/instance-methods.html#watch).

### [\#](https://v3.vuejs.org/guide/computed.html#computed-vs-watched-property)Computed vs Watched Property

Vue does provide a more generic way to observe and react to data changes
on a current active instance: watch properties. When you have some data
that needs to change based on some other data, it is tempting to overuse
watch - especially if you are coming from an AngularJS background.
However, it is often a better idea to use a computed property rather
than an imperative watch callback. Consider this example:

\<div id=\"demo\"\>{{ fullName }}\</div\>

const vm = Vue.createApp({

data() {

return {

firstName: \'Foo\',

lastName: \'Bar\',

fullName: \'Foo Bar\'

}

},

watch: {

firstName(val) {

this.fullName = val + \' \' + this.lastName

},

lastName(val) {

this.fullName = this.firstName + \' \' + val

}

}

}).mount(\'\#demo\')

The above code is imperative and repetitive. Compare it with a computed
property version:

const vm = Vue.createApp({

data() {

return {

firstName: \'Foo\',

lastName: \'Bar\'

}

},

computed: {

fullName() {

return this.firstName + \' \' + this.lastName

}

}

}).mount(\'\#demo\')

Much better, isn\'t it?

# 

# Class and Style Bindings

A common need for data binding is manipulating an element\'s class list
and its inline styles. Since they are both attributes, we can use v-bind
to handle them: we only need to calculate a final string with our
expressions. However, meddling with string concatenation is annoying and
error-prone. For this reason, Vue provides special enhancements when
v-bind is used with class and style. In addition to strings, the
expressions can also evaluate to objects or arrays.

## [\#](https://v3.vuejs.org/guide/class-and-style.html#binding-html-classes)Binding HTML Classes

### [\#](https://v3.vuejs.org/guide/class-and-style.html#object-syntax)Object Syntax

We can pass an object to :class (short for v-bind:class) to dynamically
toggle classes:

\<div :class=\"{ active: isActive }\"\>\</div\>

The above syntax means the presence of the active class will be
determined by the truthiness

(opens new window)

of the data property isActive.

You can have multiple classes toggled by having more fields in the
object. In addition, the :class directive can also co-exist with the
plain class attribute. So given the following template:

\<div

class=\"static\"

:class=\"{ active: isActive, \'text-danger\': hasError }\"

\>\</div\>

And the following data:

data() {

return {

isActive: true,

hasError: false

}

}

It will render:

\<div class=\"static active\"\>\</div\>

When isActive or hasError changes, the class list will be updated
accordingly. For example, if hasError becomes true, the class list will
become \"static active text-danger\".

The bound object doesn\'t have to be inline:

\<div :class=\"classObject\"\>\</div\>

data() {

return {

classObject: {

active: true,

\'text-danger\': false

}

}

}

This will render the same result. We can also bind to a [computed
property](https://v3.vuejs.org/guide/computed.html) that returns an
object. This is a common and powerful pattern:

\<div :class=\"classObject\"\>\</div\>

data() {

return {

isActive: true,

error: null

}

},

computed: {

classObject() {

return {

active: this.isActive && !this.error,

\'text-danger\': this.error && this.error.type === \'fatal\'

}

}

}

### [\#](https://v3.vuejs.org/guide/class-and-style.html#array-syntax)Array Syntax

We can pass an array to :class to apply a list of classes:

\<div :class=\"\[activeClass, errorClass\]\"\>\</div\>

data() {

return {

activeClass: \'active\',

errorClass: \'text-danger\'

}

}

Which will render:

\<div class=\"active text-danger\"\>\</div\>

If you would like to also toggle a class in the list conditionally, you
can do it with a ternary expression:

\<div :class=\"\[isActive ? activeClass : \'\', errorClass\]\"\>\</div\>

This will always apply errorClass, but activeClass will only be applied
when isActive is truthy.

However, this can be a bit verbose if you have multiple conditional
classes. That\'s why it\'s also possible to use the object syntax inside
array syntax:

\<div :class=\"\[{ active: isActive }, errorClass\]\"\>\</div\>

### [\#](https://v3.vuejs.org/guide/class-and-style.html#with-components)With Components

This section assumes knowledge of [Vue
Components](https://v3.vuejs.org/guide/component-basics.html). Feel free
to skip it and come back later.

When you use the class attribute on a custom component with a single
root element, those classes will be added to this element. Existing
classes on this element will not be overwritten.

For example, if you declare this component:

const app = Vue.createApp({})

app.component(\'my-component\', {

template: \`\<p class=\"foo bar\"\>Hi!\</p\>\`

})

Then add some classes when using it:

\<div id=\"app\"\>

\<my-component class=\"baz boo\"\>\</my-component\>

\</div\>

The rendered HTML will be:

\<p class=\"foo bar baz boo\"\>Hi\</p\>

The same is true for class bindings:

\<my-component :class=\"{ active: isActive }\"\>\</my-component\>

When isActive is truthy, the rendered HTML will be:

\<p class=\"foo bar active\"\>Hi\</p\>

If your component has multiple root elements, you would need to define
which component will receive this class. You can do this using \$attrs
component property:

\<div id=\"app\"\>

\<my-component class=\"baz\"\>\</my-component\>

\</div\>

const app = Vue.createApp({})

app.component(\'my-component\', {

template: \`

\<p :class=\"\$attrs.class\"\>Hi!\</p\>

\<span\>This is a child component\</span\>

\`

})

You can learn more about component attribute inheritance in the Non-Prop
[Attributes](https://v3.vuejs.org/guide/component-attrs.html) section.

## [\#](https://v3.vuejs.org/guide/class-and-style.html#binding-inline-styles)Binding Inline Styles

### [\#](https://v3.vuejs.org/guide/class-and-style.html#object-syntax-2)Object Syntax

The object syntax for :style is pretty straightforward - it looks almost
like CSS, except it\'s a JavaScript object. You can use either camelCase
or kebab-case (use quotes with kebab-case) for the CSS property names:

\<div :style=\"{ color: activeColor, fontSize: fontSize + \'px\'
}\"\>\</div\>

data() {

return {

activeColor: \'red\',

fontSize: 30

}

}

It is often a good idea to bind to a style object directly so that the
template is cleaner:

\<div :style=\"styleObject\"\>\</div\>

data() {

return {

styleObject: {

color: \'red\',

fontSize: \'13px\'

}

}

}

Again, the object syntax is often used in conjunction with computed
properties that return objects.

### [\#](https://v3.vuejs.org/guide/class-and-style.html#array-syntax-2)Array Syntax

The array syntax for :style allows you to apply multiple style objects
to the same element:

\<div :style=\"\[baseStyles, overridingStyles\]\"\>\</div\>

### [\#](https://v3.vuejs.org/guide/class-and-style.html#auto-prefixing)Auto-prefixing

When you use a CSS property that requires vendor prefixes

in :style, for example transform, Vue will automatically detect and add
appropriate prefixes to the applied styles.

### [\#](https://v3.vuejs.org/guide/class-and-style.html#multiple-values)Multiple Values

You can provide an array of multiple (prefixed) values to a style
property, for example:

\<div :style=\"{ display: \[\'-webkit-box\', \'-ms-flexbox\', \'flex\'\]
}\"\>\</div\>

This will only render the last value in the array which the browser
supports. In this example, it will render display: flex for browsers
that support the unprefixed version of flexbox.

# Conditional Rendering

## [\#](https://v3.vuejs.org/guide/conditional.html#v-if)v-if

The directive v-if is used to conditionally render a block. The block
will only be rendered if the directive\'s expression returns a truthy
value.

\<h1 v-if=\"awesome\"\>Vue is awesome!\</h1\>

It is also possible to add an \"else block\" with v-else:

\<h1 v-if=\"awesome\"\>Vue is awesome!\</h1\>

\<h1 v-else\>Oh no 😢\</h1\>

### [\#](https://v3.vuejs.org/guide/conditional.html#conditional-groups-with-v-if-on-template)Conditional Groups with v-if on \<template\>

Because v-if is a directive, it has to be attached to a single element.
But what if we want to toggle more than one element? In this case we can
use v-if on a \<template\> element, which serves as an invisible
wrapper. The final rendered result will not include the \<template\>
element.

\<template v-if=\"ok\"\>

\<h1\>Title\</h1\>

\<p\>Paragraph 1\</p\>

\<p\>Paragraph 2\</p\>

\</template\>

### [\#](https://v3.vuejs.org/guide/conditional.html#v-else)v-else

You can use the v-else directive to indicate an \"else block\" for v-if:

\<div v-if=\"Math.random() \> 0.5\"\>

Now you see me

\</div\>

\<div v-else\>

Now you don\'t

\</div\>

A v-else element must immediately follow a v-if or a v-else-if element -
otherwise it will not be recognized.

### [\#](https://v3.vuejs.org/guide/conditional.html#v-else-if)v-else-if

The v-else-if, as the name suggests, serves as an \"else if block\" for
v-if. It can also be chained multiple times:

\<div v-if=\"type === \'A\'\"\>

A

\</div\>

\<div v-else-if=\"type === \'B\'\"\>

B

\</div\>

\<div v-else-if=\"type === \'C\'\"\>

C

\</div\>

\<div v-else\>

Not A/B/C

\</div\>

Similar to v-else, a v-else-if element must immediately follow a v-if or
a v-else-if element.

## [\#](https://v3.vuejs.org/guide/conditional.html#v-show)v-show

Another option for conditionally displaying an element is the v-show
directive. The usage is largely the same:

\<h1 v-show=\"ok\"\>Hello!\</h1\>

The difference is that an element with v-show will always be rendered
and remain in the DOM; v-show only toggles the display CSS property of
the element.

v-show doesn\'t support the \<template\> element, nor does it work with
v-else.

## [\#](https://v3.vuejs.org/guide/conditional.html#v-if-vs-v-show)v-if vs v-show

v-if is \"real\" conditional rendering because it ensures that event
listeners and child components inside the conditional block are properly
destroyed and re-created during toggles.

v-if is also lazy: if the condition is false on initial render, it will
not do anything - the conditional block won\'t be rendered until the
condition becomes true for the first time.

In comparison, v-show is much simpler - the element is always rendered
regardless of initial condition, with CSS-based toggling.

Generally speaking, v-if has higher toggle costs while v-show has higher
initial render costs. So prefer v-show if you need to toggle something
very often, and prefer v-if if the condition is unlikely to change at
runtime.

## [\#](https://v3.vuejs.org/guide/conditional.html#v-if-with-v-for)v-if with v-for

Note

Using v-if and v-for together is not recommended. See the [style
guide](https://v3.vuejs.org/style-guide/#avoid-v-if-with-v-for-essential)
for further information.

When v-if and v-for are both used on the same element, v-if will be
evaluated first. See the [list rendering
guide](https://v3.vuejs.org/guide/list#v-for-with-v-if) for details.

# List Rendering

## [\#](https://v3.vuejs.org/guide/list.html#mapping-an-array-to-elements-with-v-for)Mapping an Array to Elements with v-for

We can use the v-for directive to render a list of items based on an
array. The v-for directive requires a special syntax in the form of item
in items, where items is the source data array and item is an alias for
the array element being iterated on:

\<ul id=\"array-rendering\"\>

\<li v-for=\"item in items\"\>

{{ item.message }}

\</li\>

\</ul\>

Vue.createApp({

data() {

return {

items: \[{ message: \'Foo\' }, { message: \'Bar\' }\]

}

}

}).mount(\'\#array-rendering\')

Result:

Inside v-for blocks we have full access to parent scope properties.
v-for also supports an optional second argument for the index of the
current item.

\<ul id=\"array-with-index\"\>

\<li v-for=\"(item, index) in items\"\>

{{ parentMessage }} - {{ index }} - {{ item.message }}

\</li\>

\</ul\>

Vue.createApp({

data() {

return {

parentMessage: \'Parent\',

items: \[{ message: \'Foo\' }, { message: \'Bar\' }\]

}

}

}).mount(\'\#array-with-index\')

Result:

You can also use of as the delimiter instead of in, so that it is closer
to JavaScript\'s syntax for iterators:

\<div v-for=\"item of items\"\>\</div\>

## [\#](https://v3.vuejs.org/guide/list.html#v-for-with-an-object)v-for with an Object

You can also use v-for to iterate through the properties of an object.

\<ul id=\"v-for-object\" class=\"demo\"\>

\<li v-for=\"value in myObject\"\>

{{ value }}

\</li\>

\</ul\>

Vue.createApp({

data() {

return {

myObject: {

title: \'How to do lists in Vue\',

author: \'Jane Doe\',

publishedAt: \'2016-04-10\'

}

}

}

}).mount(\'\#v-for-object\')

Result:

You can also provide a second argument for the property\'s name (a.k.a.
key):

\<li v-for=\"(value, name) in myObject\"\>

{{ name }}: {{ value }}

\</li\>

And another for the index:

\<li v-for=\"(value, name, index) in myObject\"\>

{{ index }}. {{ name }}: {{ value }}

\</li\>

Note

When iterating over an object, the order is based on the enumeration
order of Object.keys(), which isn\'t guaranteed to be consistent across
JavaScript engine implementations.

## [\#](https://v3.vuejs.org/guide/list.html#maintaining-state)Maintaining State

When Vue is updating a list of elements rendered with v-for, by default
it uses an \"in-place patch\" strategy. If the order of the data items
has changed, instead of moving the DOM elements to match the order of
the items, Vue will patch each element in-place and make sure it
reflects what should be rendered at that particular index.

This default mode is efficient, but only suitable when your list render
output does not rely on child component state or temporary DOM state
(e.g. form input values).

To give Vue a hint so that it can track each node\'s identity, and thus
reuse and reorder existing elements, you need to provide a unique key
attribute for each item:

\<div v-for=\"item in items\" :key=\"item.id\"\>

\<!\-- content \--\>

\</div\>

It is recommended to provide a key attribute with v-for whenever
possible, unless the iterated DOM content is simple, or you are
intentionally relying on the default behavior for performance gains.

Since it\'s a generic mechanism for Vue to identify nodes, the key also
has other uses that are not specifically tied to v-for, as we will see
later in the guide.

Note

Don\'t use non-primitive values like objects and arrays as v-for keys.
Use string or numeric values instead.

For detailed usage of the key attribute, please see the [key API
documentation](https://v3.vuejs.org/api/special-attributes.html#key).

## [\#](https://v3.vuejs.org/guide/list.html#array-change-detection)Array Change Detection

### [\#](https://v3.vuejs.org/guide/list.html#mutation-methods)Mutation Methods

Vue wraps an observed array\'s mutation methods so they will also
trigger view updates. The wrapped methods are:

-   push()

-   pop()

-   shift()

-   unshift()

-   splice()

-   sort()

-   reverse()

You can open the console and play with the previous examples\' items
array by calling their mutation methods. For example:
example1.items.push({ message: \'Baz\' }).

### [\#](https://v3.vuejs.org/guide/list.html#replacing-an-array)Replacing an Array

Mutation methods, as the name suggests, mutate the original array they
are called on. In comparison, there are also non-mutating methods, e.g.
filter(), concat() and slice(), which do not mutate the original array
but always return a new array. When working with non-mutating methods,
you can replace the old array with the new one:

example1.items = example1.items.filter(item =\>
item.message.match(/Foo/))1

You might think this will cause Vue to throw away the existing DOM and
re-render the entire list - luckily, that is not the case. Vue
implements some smart heuristics to maximize DOM element reuse, so
replacing an array with another array containing overlapping objects is
a very efficient operation.

## [\#](https://v3.vuejs.org/guide/list.html#displaying-filtered-sorted-results)Displaying Filtered/Sorted Results

Sometimes we want to display a filtered or sorted version of an array
without actually mutating or resetting the original data. In this case,
you can create a computed property that returns the filtered or sorted
array.

For example:

\<li v-for=\"n in evenNumbers\" :key=\"n\"\>{{ n }}\</li\>

data() {

return {

numbers: \[ 1, 2, 3, 4, 5 \]

}

},

computed: {

evenNumbers() {

return this.numbers.filter(number =\> number % 2 === 0)

}

}

In situations where computed properties are not feasible (e.g. inside
nested v-for loops), you can use a method:

\<ul v-for=\"numbers in sets\"\>

\<li v-for=\"n in even(numbers)\" :key=\"n\"\>{{ n }}\</li\>

\</ul\>

data() {

return {

sets: \[\[ 1, 2, 3, 4, 5 \], \[6, 7, 8, 9, 10\]\]

}

},

methods: {

even(numbers) {

return numbers.filter(number =\> number % 2 === 0)

}

}

## [\#](https://v3.vuejs.org/guide/list.html#v-for-with-a-range)v-for with a Range

v-for can also take an integer. In this case it will repeat the template
that many times.

\<div id=\"range\" class=\"demo\"\>

\<span v-for=\"n in 10\" :key=\"n\"\>{{ n }} \</span\>

\</div\>

Result:

## [\#](https://v3.vuejs.org/guide/list.html#v-for-on-a-template)v-for on a \<template\>

Similar to template v-if, you can also use a \<template\> tag with v-for
to render a block of multiple elements. For example:

\<ul\>

\<template v-for=\"item in items\" :key=\"item.msg\"\>

\<li\>{{ item.msg }}\</li\>

\<li class=\"divider\" role=\"presentation\"\>\</li\>

\</template\>

\</ul\>

## [\#](https://v3.vuejs.org/guide/list.html#v-for-with-v-if)v-for with v-if

TIP

Note that it\'s not recommended to use v-if and v-for together. Refer to
[style
guide](https://v3.vuejs.org/style-guide/#avoid-v-if-with-v-for-essential)
for details.

When they exist on the same node, v-if has a higher priority than v-for.
That means the v-if condition will not have access to variables from the
scope of the v-for:

\<!\-- This will throw an error because property \"todo\" is not defined
on instance. \--\>

\<li v-for=\"todo in todos\" v-if=\"!todo.isComplete\"\>

{{ todo.name }}

\</li\>

This can be fixed by moving v-for to a wrapping \<template\> tag:

\<template v-for=\"todo in todos\" :key=\"todo.name\"\>

\<li v-if=\"!todo.isComplete\"\>

{{ todo.name }}

\</li\>

\</template\>

## [\#](https://v3.vuejs.org/guide/list.html#v-for-with-a-component)v-for with a Component

This section assumes knowledge of
[Components](https://v3.vuejs.org/guide/component-basics.html). Feel
free to skip it and come back later.

You can directly use v-for on a custom component, like any normal
element:

\<my-component v-for=\"item in items\"
:key=\"item.id\"\>\</my-component\>

However, this won\'t automatically pass any data to the component,
because components have isolated scopes of their own. In order to pass
the iterated data into the component, we should also use props:

\<my-component

v-for=\"(item, index) in items\"

:item=\"item\"

:index=\"index\"

:key=\"item.id\"

\>\</my-component\>

The reason for not automatically injecting item into the component is
because that makes the component tightly coupled to how v-for works.
Being explicit about where its data comes from makes the component
reusable in other situations.

Here\'s a complete example of a simple todo list:

\<div id=\"todo-list-example\"\>

\<form v-on:submit.prevent=\"addNewTodo\"\>

\<label for=\"new-todo\"\>Add a todo\</label\>

\<input

v-model=\"newTodoText\"

id=\"new-todo\"

placeholder=\"E.g. Feed the cat\"

/\>

\<button\>Add\</button\>

\</form\>

\<ul\>

\<todo-item

v-for=\"(todo, index) in todos\"

:key=\"todo.id\"

:title=\"todo.title\"

\@remove=\"todos.splice(index, 1)\"

\>\</todo-item\>

\</ul\>

\</div\>

const app = Vue.createApp({

data() {

return {

newTodoText: \'\',

todos: \[

{

id: 1,

title: \'Do the dishes\'

},

{

id: 2,

title: \'Take out the trash\'

},

{

id: 3,

title: \'Mow the lawn\'

}

\],

nextTodoId: 4

}

},

methods: {

addNewTodo() {

this.todos.push({

id: this.nextTodoId++,

title: this.newTodoText

})

this.newTodoText = \'\'

}

}

})

app.component(\'todo-item\', {

template: \`

\<li\>

{{ title }}

\<button \@click=\"\$emit(\'remove\')\"\>Remove\</button\>

\</li\>

\`,

props: \[\'title\'\],

emits: \[\'remove\'\]

})

app.mount(\'\#todo-list-example\')

# Shared Components

### Admin Sidebar

#### Admin Routes (js)

#### Admin Sidebar (vue)

#### Menu Item (vue)

# Functions

### API

### Organizations Services (js)

### Types Services (js)

### API services (js)

### 

### Constants (js)

Declare constants in a separate constants.js file which we can require
into the other Vue component:

-   Sustainable Development Goals(SDG) Codes

-   SDG labels

-   SDG Colors

-   Months

-   Media file Upload Constraints

### Dotatlas (js)

dotAtlas is a JavaScript library for interactive exploration of 2d point
collections. dotAtlas can produce zoomable visualizations similar to the
one shown below. They combine various types of layers, such as
elevations, markers or labels, to produce an attractive map-like
presentation of your data.

![Result of the quick start simple dotAtlas
visualization.](media/image2.jpg){width="5.111111111111111in"
height="1.9027777777777777in"}

There are three ways to get started with dotAtlas:

-   [[Quick
    > start]{.ul}](https://get.carrotsearch.com/dotatlas/latest/doc/quick-start/):
    > setting up your first simple dotAtlas visualization with a minimal
    > amount of code.

-   Guides: in-depth articles covering various aspects of dotAtlas, such
    > as
    > [[requirements]{.ul}](https://get.carrotsearch.com/dotatlas/latest/doc/requirements/),
    > [[installation]{.ul}](https://get.carrotsearch.com/dotatlas/latest/doc/installation/),
    > [[API
    > overview]{.ul}](https://get.carrotsearch.com/dotatlas/latest/doc/api-overview/),
    > [[defining
    > layers]{.ul}](https://get.carrotsearch.com/dotatlas/latest/doc/defining-layers/),
    > [[listening to
    > events]{.ul}](https://get.carrotsearch.com/dotatlas/latest/doc/listening-to-events/)
    > and more.

-   [[Tutorial]{.ul}](https://get.carrotsearch.com/dotatlas/latest/doc/tutorial/):
    > step by step instructions on building a more complex dotAtlas
    > visualization, including: layer set-up, handling user interactions
    > and implementing hover and selection highlights.

Finally, the
[[API]{.ul}](https://get.carrotsearch.com/dotatlas/latest/doc/api-common/)
[[references]{.ul}](https://get.carrotsearch.com/dotatlas/latest/doc/api-dotatlas/)
contain details on all the available options and methods.

### Functions (js)

Key functions that export the authorization and authentication of the
user and provide appropriate privileges including project edit, publish
& review rights to the user and relevant project(s).

# Admin Pages

# Window Components

## Application Dialogs

Gallery

VideoProvider

## Mini Windows

## Popup Windows

# Translation Files

# Routing

# Transitions & Animations

# External Libraries

### Vue.js

\[Vue.js\](https://vuejs.org/) is a javascript web framework.

### TipTap

\[TipTap\](https://github.com/ueberdosis/tiptap) is a toolkit for
building text editors. We are using the vue package for TipTap. TipTap
is an extension to \[ProseMirror\](https://prosemirror.net/) that allows
you to create new schemas directly in a vue way.

This editor is used to edit a project\'s description or blog post.

### Vue Leaflet

\[Vue Leaflet\](https://vue2-leaflet.netlify.app/) is a vue package
built on Leaflet.

Leaflet is a strong package to build maps and interact with it.

### Vue Color

\[Vue Color\](https://github.com/xiaokaike/vue-color) is a vue color
picker package. It provides a different picker from simple hex code to
color choice with opacity.

We are using it to let organization administrators select a background
color for categories.

### Axios

\[Axios\](https://github.com/axios/axios) is an Http client.

We are using it to manage HTTP calls to our API. It is based on promise.

### Drag and resize

\[vue-drag-resize\](https://github.com/kirillmurashov/vue-drag-resize)
is a package made for image resizing and dragging.

We are using it on blog post and description when user upload images or
videos

### Bulma

\[Bulma\](https://bulma.io/) is a CSS framework. We are using the basic
version for responsibility and basic component class : Button, Grid etc.

We are also using some components of \[Bulma
extension\](https://bulma.io/extensions/) that bring css/js components
like tooltip.

### ChartJs

\[vue-chartjs\](https://vue-chartjs.org/) is a vue wrapper to Chart.js

We are using it to build chart in Stats page

# State Management

# Server side Rendering
