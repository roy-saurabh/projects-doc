#


[Installation](#_fn6bu2gvbzqd)

[Architecture](#_9oe3cg2coeto)

[Release Notes](#_5v1ba8l5ugip)

[Frontend - Home](#_vs8nrd2bqdbe)

[Backend - Home](#_75rsxi7hkyu0)

[Database](#_e9vpbkuljk9n)

[Create Operations](#_s67o33bgu3c)

[Read Operations](#_sjr1aocd7f5a)

[Update Operations](#_skly48dewuxk)

[Delete Operations](#_rc7ufd2iy353)

[Bulk Write](#_hd32tn50511j)

[Versioning](#_90zc2yyomjdk)

[Key relevant GitLab documentation](#_2fsmqzb6mnjj)

[Popular topics](#_wzdgwja1q87l)

[The entire DevOps lifecycle](#_djl7qdslnk5g)

[Introduction](#_xf76c6dp1j4p)

[Helping the community](#_82ruq0qb9mlg)

[Communicate better](#_nab8u87bjetg)

[What fields are included in a project?](#_j6fbzbgrnaen)

[What is a Projects Platform?](#_2xnvddzasb9m)

[Getting Started](#_8gsrwucni4xd)

[Our current Projects platform folder structure](#_tasuif700vwx)

[Key Folders](#_sjwzx5cfg5oq)

[Application Dialogs (appdialogs)](#_jnllcib7fkjk)

[Assets (assets)](#_ueowqkjqe11m)

[Global Functions (functs)](#_evk2isqnvxbn)

[Mixins (mixins)](#_grahqs6dh453)

[Mini Pop-in Windows(miniwins)](#_m603lypgeh8)

[Pages (pages)](#_astvp4toexnp)

[Popups (popups)](#_mnhfak18clbn)

[SCSS (scss)](#_hdqbv8w3gwhk)

[Shared Components (shrcomponents)](#_73ixqvakwebx)

[Windows (wins)](#_ieaaqbgnbjxy)

[Custom Vue Event Bus (VBUS)](#_9lf559lkzuez)

[Application &amp; Component Instances](#_8mwp277kdbpp)

[Creating an Application Instance](#_7tbuu1syh0q4)

[#The Root Component](#_rmt8l8omdy41)

[#Component Instance Properties](#_u71pa4x5femg)

[#Lifecycle Hooks](#_je6azz1grbkn)

[#Lifecycle Diagram](#_xdx8f6uv7s3w)

[Template Syntax](#_vpkcvoowy38m)

[#Interpolations](#_a51d2tq2kk7k)

[#Text](#_o4uwuuxehavw)

[#Raw HTML](#_mtbvcgqber82)

[#Attributes](#_9amrir5ypnxi)

[#Using JavaScript Expressions](#_n9j9dzqj8dcs)

[#Directives](#_wygfp82ubjz8)

[#Arguments](#_7her7pafi7rf)

[#Dynamic Arguments](#_pzvcr0cu7y2d)

[#Modifiers](#_noefgkwg128d)

[#Shorthands](#_kzftareaaih)

[#Caveats](#_jsgvv4hsfrge)

[#Dynamic Argument Value Constraints](#_9wt4n4g4jbqq)

[#Dynamic Argument Expression Constraints](#_jnh06vtspc4v)

[Data Properties and Methods](#_y1qflc8pfunh)

[#Data Properties](#_puazugisnhkv)

[#Methods](#_2bwzac41snj6)

[Computed Properties and Watchers](#_ve49nmce3i1r)

[#Computed Properties](#_ijz8hjdh77m0)

[#Basic Example](#_x4tkzn6yk09o)

[#Computed Caching vs Methods](#_mcdtys44khnd)

[#Computed Setter](#_d4cf3fvpy9nz)

[#Watchers](#_18lt178pax3n)

[#Computed vs Watched Property](#_rnpbsc1wm7)

[Class and Style Bindings](#_23j6we7q8w9d)

[#Binding HTML Classes](#_m3h87wzh99s2)

[#Object Syntax](#_h44jgyq02vs2)

[#Array Syntax](#_psm7sgqd6rct)

[#With Components](#_ef6zu16t7tfs)

[#Binding Inline Styles](#_y1j7sahy41n7)

[#Object Syntax](#_sw7oktigeo6)

[#Array Syntax](#_ts4n0sp3ovaj)

[#Auto-prefixing](#_xs8xeg27xp40)

[#Multiple Values](#_av9e04bxfxu6)

[Conditional Rendering](#_6c4fhh7ea41w)

[#v-if](#_6ih6f3ragzhe)

[#Conditional Groups with v-if on \&lt;template\&gt;](#_sl2nxps88lv7)

[#v-else](#_1nd3lz6mwcjl)

[#v-else-if](#_jwd44ixzkls0)

[#v-show](#_6sxxab8ux9y7)

[#v-if vs v-show](#_xmgak534vmwr)

[#v-if with v-for](#_5mpgededv75z)

[List Rendering](#_crp91cor6rmg)

[#Mapping an Array to Elements with v-for](#_1zfyp2p7jywg)

[#v-for with an Object](#_bgx8bzb2c44s)

[#Maintaining State](#_z23z3bv1ezbv)

[#Array Change Detection](#_b7afhx7gto5y)

[#Mutation Methods](#_10j204akafrm)

[#Replacing an Array](#_sft36h2in7zb)

[#Displaying Filtered/Sorted Results](#_5siycxnm1g39)

[#v-for with a Range](#_3aqck2txee0v)

[#v-for on a \&lt;template\&gt;](#_9sc0lckqr28c)

[#v-for with v-if](#_nbcmpp1nudrx)

[#v-for with a Component](#_7b2zv5sua9se)

[Main Files](#_gmrxgjtv6wun)

[App.vue](#_thxmcj7kt994)

[Miniwin.vue](#_p1kxku1wp8k)

[Msg.vue](#_wrsspq7h2v9d)

[BigWin.vue](#_pz08xd3k69d7)

[TopBar.vue](#_iphjh8ew8umw)

[Main.css](#_1y86pr6sqjjj)

[Main.js](#_3d0ojf8zryhh)

[Router.js](#_ai39ptn4l8is)

[AppDialog.vue](#_regzstuly8jb)

[PopUp.vue](#_b949qsw5z1w7)

[Shared Components](#_4gsinovwrlqe)

[Admin Sidebar](#_v5rdv111isj)

[Admin Routes (js)](#_251iuf43ptm)

[Admin Sidebar (vue)](#_251iuf43ptm)

[Menu Item (vue)](#_251iuf43ptm)

[Functions](#_txco1thp5xs3)

[API](#_1438y3ug97sv)

[Organizations Services (js)](#_1438y3ug97sv)

[Types Services (js)](#_1438y3ug97sv)

[API services (js)](#_1438y3ug97sv)

[Constants (js)](#_qz8r382gii3g)

[Dotatlas (js)](#_1438y3ug97sv)

[Functions (js)](#_1438y3ug97sv)

[Pages](#_lsqzd6uzjjbl)

[Admin Pages](#_pe03b6e9ge34)

[Sub Pages - Components](#_5k455kcjapmi)

[Main Pages - Components](#_cuc2efcfok4)

[Window Components](#_20dezsjrhj1o)

[Application Dialogs](#_xuz996nnqeed)

[Gallery.vue](#_ul87lpqh9or2)

[VideoProviderChooser.vue](#_yk5ugtezzzs)

[Mini Windows](#_802rxh6it6yk)

[Copy.vue](#_wkd79utu6a06)

[CopyLink.vue](#_yyo2x0ub2mmj)

[EditResFile.vue](#_h2ydlkce6j2b)

[Edit ResLink.vue](#_oqy2dxxmql0k)

[EditResProject.vue](#_fhy3oqtfmi0k)

[MiniInfo.vue](#_mm1tssj5my2u)

[UnsavedData.vue](#_6676kh1c7907)

[YesNo.vue](#_u0in08qb20et)

[Popup Windows](#_kkhpj3ffy705)

[Translation Files](#_asfcy323du7l)

[Routing](#_83qvpabk2657)

[Transitions &amp; Animations](#_h2r990raxsep)

[External Libraries](#_ws7g7pbljxc4)

[Vue.js](#_4a284pldl9jx)

[TipTap](#_ly4kf5peeh68)

[Vue Leaflet](#_9fv1nae4wfvl)

[Vue Color](#_pvw7hc63laaz)

[Axios](#_2sfzplde2vwn)

[Drag and resize](#_43ncb6ji1f9a)

[Bulma](#_k9kygo6jujxt)

[ChartJs](#_fn0zypbty2bm)

[State Management](#_8aun7m4i0kvl)

[Server side Rendering](#_uwqa83m4xm6y)

[Backend APIs](#_fz2cvbcl63z6)

[### api](#_kssnaikc50sq)

[### Authentication](#_hx0ycrrcpn1k)

[### api\_cstm](#_n1ot6cuy1qs3)

[### api\_funct](#_m1w2i9gzyyn8)

[### api\_private](#_kg7481hfmn2z)

[### ref](#_bjvmy36y26ms)

[### settings](#_qnw6ify3grb6)

[### migrations](#_l9m77ecyz1ix)

[### exceptions](#_twwj576xqkvm)

[### TPL](#_bsj2sml1ezcg)

#


#
# Installation

Currently there are a lot of dependencies required for a Projects Platform development environment and managing complexity around building Projects Platform Frontend, Backend, CRI People interface, Sockets etc. To mitigate the complexity, we decided to build LXC containers to create a complete environment with all dependencies pre-configured to start contributing to the Projects Platform code in the shortest possible time.

We replicate the environmental configuration to build a pre-production environment too and make an ISO environment for pre-production and production environment with built-in scripts and access.

1. Create a [SSH key](https://www.ssh.com/ssh/key/) and share the public key with the core user group member with Projects Platform application environment admin access on the main development server.
2. The admin would add the public key in authorized\_keys file and would create a development environment for the Projects Platform application that you would now be able to connect to with the provided SSH address _(e.g. : `ssh dev@dev.cri-paris.org -p :\&lt;\&lt;port#\&gt;\&gt;`)._
3. Access the directory and explore code folders containing frontend code at `/WWW/DEV/FRONT` or backend code at `/WWW/DEV/BACK`.
4. Install any IDE of your choice and install either SSH tools to connect from your computer to the remote server or nautilus configuration. (OS dependent)

## Architecture

The Projects Platform API server is developed in Python using the Flask micro framework. The data &amp; state of the platform are stored in MongoDB. Socket.IO server running under python enables real-time, bidirectional and event-based communication. The client side rendering of DOM of the Project application leverages VueJS and synchronous interactions are managed by the socket.io and prosemirror client libraries.

## Release Notes

Latest version: **v0.13.1**

Detailed release notes for each version are available on [GitLab](https://git.cri-paris.org/it-team/project/projects-front/-/tree/release_v0.13.1)

### Frontend - Home

### run FRONT

1. Go to `/WWW/FRONT`
2. Run `npm run dev` your web application will be available on `_https://dev.cri-paris.org:\&lt;\&lt;port#\&gt;\&gt;_` Change with the right port of your env !
3. Constants are in `dist/const.js` Some are set up within the env creation. For more details go [here](front/constants.md)

### Backend - Home

### run BACK

1. The backend is already running!
2. If something went wrong and you need to re-launch the back process: &#39;_sudo touch /etc/uwsgi-emperor/vassals/apiprojectsdev.ini_&#39;. This command needs to be run after any modification of &#39;settings.py&#39;.
3. Access logs: &#39;_sudo tail -f /var/log/uwsgi/vassals/apiprojectsdev.log_&#39;.
4. Constants are in &#39;_/const.py_&#39; Some are set up within the env creation. For more details go &#39;_back/constants.md_&#39;.

### Database

### run MONGO

MongoDB CRUD operations create, read, update, and delete dB documents:

1. To access Mongo CRUD operations, modify dB.
2. Just run `mongo`.
3. Choose the right DB (default: &#39;_apiprojectsdev_&#39;) using &#39;use&#39;.
4. Start querying using common commands [here](https://docs.mongodb.com/manual/reference/mongo-shell/)

#### Create Operations

Create or insert operations add new [documents](https://docs.mongodb.com/manual/core/document/#bson-document-format) to a [collection](https://docs.mongodb.com/manual/core/databases-and-collections/#collections). If the collection does not currently exist, insert operations will create the collection.

MongoDB provides the following methods to insert documents into a collection:

- [db.collection.insertOne()](https://docs.mongodb.com/manual/reference/method/db.collection.insertOne/#db.collection.insertOne)_New in version 3.2_
- [db.collection.insertMany()](https://docs.mongodb.com/manual/reference/method/db.collection.insertMany/#db.collection.insertMany)_New in version 3.2_

In MongoDB, insert operations target a single [collection](https://docs.mongodb.com/manual/reference/glossary/#term-collection). All write operations in MongoDB are [atomic](https://docs.mongodb.com/manual/core/write-operations-atomicity/) on the level of a single [document](https://docs.mongodb.com/manual/core/document/).

For examples, see [Insert Documents](https://docs.mongodb.com/manual/tutorial/insert-documents/).

#### Read Operations

Read operations retrieve [documents](https://docs.mongodb.com/manual/core/document/#bson-document-format) from a [collection](https://docs.mongodb.com/manual/core/databases-and-collections/#collections); i.e. query a collection for documents. MongoDB provides the following methods to read documents from a collection:

- [db.collection.find()](https://docs.mongodb.com/manual/reference/method/db.collection.find/#db.collection.find)

You can specify [query filters or criteria](https://docs.mongodb.com/manual/tutorial/query-documents/#read-operations-query-argument) that identify the documents to return.

For examples, see:

- [Query Documents](https://docs.mongodb.com/manual/tutorial/query-documents/)
- [Query on Embedded/Nested Documents](https://docs.mongodb.com/manual/tutorial/query-embedded-documents/)
- [Query an Array](https://docs.mongodb.com/manual/tutorial/query-arrays/)
- [Query an Array of Embedded Documents](https://docs.mongodb.com/manual/tutorial/query-array-of-documents/)

#### Update Operations

Update operations modify existing [documents](https://docs.mongodb.com/manual/core/document/#bson-document-format) in a [collection](https://docs.mongodb.com/manual/core/databases-and-collections/#collections). MongoDB provides the following methods to update documents of a collection:

- [db.collection.updateOne()](https://docs.mongodb.com/manual/reference/method/db.collection.updateOne/#db.collection.updateOne)_New in version 3.2_
- [db.collection.updateMany()](https://docs.mongodb.com/manual/reference/method/db.collection.updateMany/#db.collection.updateMany)_New in version 3.2_
- [db.collection.replaceOne()](https://docs.mongodb.com/manual/reference/method/db.collection.replaceOne/#db.collection.replaceOne)_New in version 3.2_

In MongoDB, update operations target a single collection. All write operations in MongoDB are [atomic](https://docs.mongodb.com/manual/core/write-operations-atomicity/) on the level of a single document.

You can specify criteria, or filters, that identify the documents to update. These [filters](https://docs.mongodb.com/manual/core/document/#document-query-filter) use the same syntax as read operations.

For examples, see [Update Documents](https://docs.mongodb.com/manual/tutorial/update-documents/).

#### Delete Operations

Delete operations remove documents from a collection. MongoDB provides the following methods to delete documents of a collection:

- [db.collection.deleteOne()](https://docs.mongodb.com/manual/reference/method/db.collection.deleteOne/#db.collection.deleteOne)_New in version 3.2_
- [db.collection.deleteMany()](https://docs.mongodb.com/manual/reference/method/db.collection.deleteMany/#db.collection.deleteMany)_New in version 3.2_

In MongoDB, delete operations target a single [collection](https://docs.mongodb.com/manual/reference/glossary/#term-collection). All write operations in MongoDB are [atomic](https://docs.mongodb.com/manual/core/write-operations-atomicity/) on the level of a single document.

You can specify criteria, or filters, that identify the documents to remove. These [filters](https://docs.mongodb.com/manual/core/document/#document-query-filter) use the same syntax as read operations.

For examples, see [Delete Documents](https://docs.mongodb.com/manual/tutorial/remove-documents/).

#### Bulk Write

MongoDB provides the ability to perform write operations in bulk. For details, see [Bulk Write Operations](https://docs.mongodb.com/manual/core/bulk-write-operations/).

### Versioning

### GIT

Here you can access the complete documentation for GitLab, the single application for the [entire DevOps lifecycle](https://docs.gitlab.com/ee/README.html#the-entire-devops-lifecycle).

#### Key relevant GitLab documentation

| **Essential documentation** | **Essential documentation** |
| --- | --- |
| [User documentation](https://docs.gitlab.com/ee/user/index.html)Discover features and concepts for GitLab users. | [Administrator documentation](https://docs.gitlab.com/ee/administration/index.html)Everything GitLab self-managed administrators need to know. |
| [Contributing to GitLab](https://docs.gitlab.com/ee/README.html#contributing-to-gitlab)At GitLab, everyone can contribute! | [New to Git and GitLab?](https://docs.gitlab.com/ee/README.html#new-to-git-and-gitlab)We have the resources to get you started. |
| [Build an integration with GitLab](https://docs.gitlab.com/ee/README.html#build-an-integration-with-gitlab)Consult our integration documentation. | [Coming to GitLab from another platform?](https://docs.gitlab.com/ee/README.html#coming-to-gitlab-from-another-platform)Consult our guides. |
| [Install GitLab](https://about.gitlab.com/install/)Installation options for different platforms. | [Customers](https://docs.gitlab.com/ee/subscriptions/index.html)Information for new and existing customers. |
| [Update GitLab](https://docs.gitlab.com/ee/update/index.html)Update your GitLab self-managed instance to the latest version. | [Reference Architectures](https://docs.gitlab.com/ee/administration/reference_architectures/index.html)GitLab reference architectures. |
| [GitLab releases](https://about.gitlab.com/releases/)What&#39;s new in GitLab. | |

#### Popular topics

Have a look at some of our most popular topics:

| **Popular topic** | **Description** |
| --- | --- |
| [Two-factor authentication](https://docs.gitlab.com/ee/user/profile/account/two_factor_authentication.html) | Improve the security of your GitLab account. |
| [GitLab groups](https://docs.gitlab.com/ee/user/group/index.html) | Manage projects together. |
| [GitLab CI/CD pipeline configuration reference](https://docs.gitlab.com/ee/ci/yaml/README.html) | Available configuration options for .gitlab-ci.yml files. |
| [Activate GitLab EE with a license](https://docs.gitlab.com/ee/user/admin_area/license.html) | Activate GitLab Enterprise Edition functionality with a license. |
| [Back up and restore GitLab](https://docs.gitlab.com/ee/raketasks/backup_restore.html) | Rake tasks for backing up and restoring GitLab self-managed instances. |
| [GitLab release and maintenance policy](https://docs.gitlab.com/ee/policy/maintenance.html) | Policies for version naming and cadence, and also upgrade recommendations. |
| [Elasticsearch integration](https://docs.gitlab.com/ee/integration/elasticsearch.html) | Integrate Elasticsearch with GitLab to enable advanced searching. |
| [Omnibus GitLab database settings](https://docs.gitlab.com/omnibus/settings/database.html) | Database settings for Omnibus GitLab self-managed instances. |
| [Omnibus GitLab NGINX settings](https://docs.gitlab.com/omnibus/settings/nginx.html) | NGINX settings for Omnibus GitLab self-managed instances. |
| [Omnibus GitLab SSL configuration](https://docs.gitlab.com/omnibus/settings/ssl.html) | SSL settings for Omnibus GitLab self-managed instances. |
| [GitLab.com settings](https://docs.gitlab.com/ee/user/gitlab_com/index.html) | Settings used for GitLab.com. |

#### The entire DevOps lifecycle

GitLab is the application for software development, security, and operations that enables [Concurrent DevOps](https://about.gitlab.com/topics/concurrent-devops/). GitLab makes the software lifecycle faster and radically improves the speed of business. Git is directly configured so you can add your own gitlab CRI alias and start creating your own feature branch.

# Introduction

Projects platform to reference a community&#39;s projects and is home to a community of passionate, inspiring projects that are launched there every day.

Nevertheless, it is difficult to know what is going on there every day, and we all &quot;miss&quot; many daily achievements. Because of a lack of visibility, some projects lose the opportunity for better support, and precious resources are spent on redundant ideas.

### Helping the community

We believe that it will also make it easier to train teams on certain subjects by allowing them to better identify the skills and achievements already available or in gestation.

It is also a way to get to know the people in the community or who revolve around the organization and its projects, in line with the objectives of sustainable development defined by the United Nations.

### Communicate better

This platform will enhance the organization&#39;s impact by simply presenting the extent of its creative force and potential.

This will benefit everyone, with each project benefiting from centralized and broader communication.

Indeed Projects Platform is, as well as CRI people, a data source for all CRI&#39;s digital means of communication, avoiding - badly - duplicated information.

### What fields are included in a project?

When you create a new project, you create a title, an image, contributors and you can annotate it by UNESCO&#39;s sustainable development objectives to which it is addressed and by keywords. These keywords are chosen from all available Wikipedia article titles. They make it easy to find projects with similarities. In the following, they will also be visualized and shared on the WeLearn cartography.

## What is a Projects Platform?

In order to better share ideas worth sharing with everyone, we have created the Projects platform for presentation and referencing of all projects that are intended to be collaborative and easy to access, it will allow everyone to have a directory of the many projects carried out and to present their own achievements.

We also believe that other organizations have the same need for better project sharing. We propose that they benefit from this tool.

### Getting Started

#### Our current Projects platform folder structure

#### **Key Folders**

##### Application Dialogs (appdialogs)

Pop-in component for Description and Blog. Vue component inside should be moved in shrcomponents or wins

##### Assets (assets)

Fonts and global images. Warning : Images are now in a file system based so no new images should be added here and the /img subfolder might be deleted.

##### Global Functions (functs)

Global function that can be reused. It should contain services. Some functions might be added in a mixin.

##### Mixins (mixins)

Component function that can be added in more than one component. Refers to vue documentation to understand the meaning of a mixin.

##### Mini Pop-in Windows(miniwins)

Small pop-in component. It would be better to have few functional pop-in component and inject only text in it.

##### Pages (pages)

It should only contain user pages and those pages components should be built with other component.

##### Popups (popups)

Popup components

##### SCSS (scss)

SCSS global files

##### Shared Components (shrcomponents)

All reusable components. All components expect pages and one used component should be here. Even wins and miniwins.

##### Windows (wins)

Large pop-in components

#### **Custom Vue Event Bus (VBUS)**

To understand VBUS is critical to understand Projects Platform component event communication. We currently don&#39;t use Vuex that could be a better way to manage state and data flow across components. We are utilizing VBUS currently to connect unrelated sections of our VueJs Application/Codebase talk to each other with current project code event bus/publisher-subscriber pattern. The same has provided flexibility to have communication between unrelated or sibling relationships but can very easily create ambiguous and unmanageable state management within an application as complex as the Projects Platform. So the next stage of optimization of Projects would include re-architecting the application and include Vuex to alter a global state that all components check for via getters instead of VBUS.

So then in a completely unrelated component you would need to hook into that event and react to it, I find myself registering the event hooks in the components mounted() lifecycle hook to be able to listen to events. Similar to child to parent communication but the difference is the component reacting to the event registers its listener in a different place (in this case in the mounted hook). Now you have the ability for one component to speak to another component in a different part of your application. It is a handy thing to know but of course beware of overusing this. It could get mucky or used where a different approach might better suit. So these event systems come part and parcel of Vue and can be utilised to achieve component communication in a variety of ways.

The Publisher-Subscriber pattern we will use to allow components to subscribe to an event. Then other components can publish an event and all subscribers can then react to that. Two main methods to allow subscription and the ability to publish to those subscribers. Again this then means we get access in every component to the PubSub instance via this.$pubSub. So then we must subscribe to some components, a good example would be a bunch of show/hide panel components, they all can open independently. You wish to have a button elsewhere in the application that you would want to have the ability to close all those other panel components with one click. So here we see that we will use mounted() to subscribe to an event called closePanels. When it is invoked then we will run our localMethod to close the panel. So this time our click event will run this. $pubSub.publish(&#39;closePanels&#39;), which will inform all subscribers to run and thus close them all. We have run through different ways to utilise communication throughout your VueJs Application. We have used event systems and we have used some patterns to help the way these components communicate. Again it is trying to find the right time to use each and when.

# Application &amp; Component Instances

## Creating an Application Instance

Every Vue application starts by creating a new application instance with the createApp function:

const app = Vue.createApp({

/\* options \*/

})

The application instance is used to register &#39;globals&#39; that can then be used by components within that application. We&#39;ll discuss that in detail later in the guide but as a quick example:

const app = Vue.createApp({})

app.component(&#39;SearchInput&#39;, SearchInputComponent)

app.directive(&#39;focus&#39;, FocusDirective)

app.use(LocalePlugin)

Most of the methods exposed by the application instance return that same instance, allowing for chaining:

Vue.createApp({})

.component(&#39;SearchInput&#39;, SearchInputComponent)

.directive(&#39;focus&#39;, FocusDirective)

.use(LocalePlugin)

You can browse the full application API in the [API reference](https://v3.vuejs.org/api/application-api.html).

## [#](https://v3.vuejs.org/guide/instance.html#the-root-component)The Root Component

The options passed to createApp are used to configure the root component. That component is used as the starting point for rendering when we mount the application.

An application needs to be mounted into a DOM element. For example, if we want to mount a Vue application into \&lt;div id=&quot;app&quot;\&gt;\&lt;/div\&gt;, we should pass #app:

const RootComponent = {

/\* options \*/

}

const app = Vue.createApp(RootComponent)

const vm = app.mount(&#39;#app&#39;)

Unlike most of the application methods, mount does not return the application. Instead it returns the root component instance.

Although not strictly associated with the [MVVM pattern](https://en.wikipedia.org/wiki/Model_View_ViewModel), Vue&#39;s design was partly inspired by it. As a convention, we often use the variable vm (short for ViewModel) to refer to a component instance.

While all the examples on this page only need a single component, most real applications are organized into a tree of nested, reusable components. For example, a Todo application&#39;s component tree might look like this:

Root Component

└─ TodoList

├─ TodoItem

│ ├─ DeleteTodoButton

│ └─ EditTodoButton

└─ TodoListFooter

├─ ClearTodosButton

└─ TodoListStatistics

Each component will have its own component instance, vm. For some components, such as TodoItem, there will likely be multiple instances rendered at any one time. All of the component instances in this application will share the same application instance.

We&#39;ll talk about [the component system](https://v3.vuejs.org/guide/component-basics.html) in detail later. For now, just be aware that the root component isn&#39;t really any different from any other component. The configuration options are the same, as is the behavior of the corresponding component instance.

## [#](https://v3.vuejs.org/guide/instance.html#component-instance-properties)Component Instance Properties

Earlier in the guide we met data properties. Properties defined in data are exposed via the component instance:

const app = Vue.createApp({

data() {

return { count: 4 }

}

})

const vm = app.mount(&#39;#app&#39;)

console.log(vm.count) // =\&gt; 4

There are various other component options that add user-defined properties to the component instance, such as methods, props, computed, inject and setup. We&#39;ll discuss each of these in depth later in the guide. All of the properties of the component instance, no matter how they are defined, will be accessible in the component&#39;s template.

Vue also exposes some built-in properties via the component instance, such as $attrs and $emit. These properties all have a $ prefix to avoid conflicting with user-defined property names.

## [#](https://v3.vuejs.org/guide/instance.html#lifecycle-hooks)Lifecycle Hooks

Each component instance goes through a series of initialization steps when it&#39;s created - for example, it needs to set up data observation, compile the template, mount the instance to the DOM, and update the DOM when data changes. Along the way, it also runs functions called lifecycle hooks, giving users the opportunity to add their own code at specific stages.

For example, the [created](https://v3.vuejs.org/api/options-lifecycle-hooks.html#created) hook can be used to run code after an instance is created:

Vue.createApp({

data() {

return { count: 1 }

},

created() {

// `this` points to the vm instance

console.log(&#39;count is: &#39; + this.count) // =\&gt; &quot;count is: 1&quot;

}

})

There are also other hooks which will be called at different stages of the instance&#39;s lifecycle, such as [mounted](https://v3.vuejs.org/api/options-lifecycle-hooks.html#mounted), [updated](https://v3.vuejs.org/api/options-lifecycle-hooks.html#updated), and [unmounted](https://v3.vuejs.org/api/options-lifecycle-hooks.html#unmounted). All lifecycle hooks are called with this context pointing to the current active instance invoking it

Don&#39;t use [arrow functions](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Functions/Arrow_functions)on an options property or callback, such as created: () =\&gt; console.log(this.a) or vm.$watch(&#39;a&#39;, newValue =\&gt; this.myMethod()). Since an arrow function doesn&#39;t have a this, this will be treated as any other variable and lexically looked up through parent scopes until found, often resulting in errors such as Uncaught TypeError: Cannot read property of undefined or Uncaught TypeError: this.myMethod is not a function.

## [#](https://v3.vuejs.org/guide/instance.html#lifecycle-diagram)Lifecycle Diagram

Below is a diagram for the instance lifecycle. You don&#39;t need to fully understand everything going on right now, but as you learn and build more, it will be a useful reference. ![](RackMultipart20210310-4-fcaz0h_html_381214b743fb8be9.png)

# Template Syntax

Vue.js uses an HTML-based template syntax that allows you to declaratively bind the rendered DOM to the underlying component instance&#39;s data. All Vue.js templates are valid HTML that can be parsed by spec-compliant browsers and HTML parsers.

Under the hood, Vue compiles the templates into Virtual DOM render functions. Combined with the reactivity system, Vue is able to intelligently figure out the minimal number of components to re-render and apply the minimal amount of DOM manipulations when the app state changes.

If you are familiar with Virtual DOM concepts and prefer the raw power of JavaScript, you can also [directly write render functions](https://v3.vuejs.org/guide/render-function.html) instead of templates, with optional JSX support.

## [#](https://v3.vuejs.org/guide/template-syntax.html#interpolations)Interpolations

### [#](https://v3.vuejs.org/guide/template-syntax.html#text)Text

The most basic form of data binding is text interpolation using the &quot;Mustache&quot; syntax (double curly braces):

\&lt;span\&gt;Message: {{ msg }}\&lt;/span\&gt;

The mustache tag will be replaced with the value of the msg property from the corresponding component instance. It will also be updated whenever the msg property changes.

You can also perform one-time interpolations that do not update on data change by using the [v-once directive](https://v3.vuejs.org/api/directives.html#v-once), but keep in mind this will also affect any other bindings on the same node:

\&lt;span v-once\&gt;This will never change: {{ msg }}\&lt;/span\&gt;

### [#](https://v3.vuejs.org/guide/template-syntax.html#raw-html)Raw HTML

The double mustaches interpret the data as plain text, not HTML. In order to output real HTML, you will need to use the [v-html](https://v3.vuejs.org/api/directives.html#v-html)[directive](https://v3.vuejs.org/api/directives.html#v-html):

\&lt;p\&gt;Using mustaches: {{ rawHtml }}\&lt;/p\&gt;

\&lt;p\&gt;Using v-html directive: \&lt;span v-html=&quot;rawHtml&quot;\&gt;\&lt;/span\&gt;\&lt;/p\&gt;

The contents of the span will be replaced with the value of the rawHtml property, interpreted as plain HTML - data bindings are ignored. Note that you cannot use v-html to compose template partials, because Vue is not a string-based templating engine. Instead, components are preferred as the fundamental unit for UI reuse and composition.

TIP

Dynamically rendering arbitrary HTML on your website can be very dangerous because it can easily lead to XSS vulnerabilities

. Only use HTML interpolation on trusted content and never on user-provided content

### [#](https://v3.vuejs.org/guide/template-syntax.html#attributes)Attributes

Mustaches cannot be used inside HTML attributes. Instead, use a [v-bind](https://v3.vuejs.org/api/directives.html#v-bind)[directive](https://v3.vuejs.org/api/directives.html#v-bind):

\&lt;div v-bind:id=&quot;dynamicId&quot;\&gt;\&lt;/div\&gt;

If the bound value is null or undefined then the attribute will not be included on the rendered element.

In the case of boolean attributes, where their mere existence implies true, v-bind works a little differently. For example:

\&lt;button v-bind:disabled=&quot;isButtonDisabled&quot;\&gt;Button\&lt;/button\&gt;

The disabled attribute will be included if isButtonDisabled has a truthy value. It will also be included if the value is an empty string, maintaining consistency with \&lt;button disabled=&quot;&quot;\&gt;. For other falsy values the attribute will be omitted.

### [#](https://v3.vuejs.org/guide/template-syntax.html#using-javascript-expressions)Using JavaScript Expressions

So far we&#39;ve only been binding to simple property keys in our templates. But Vue.js actually supports the full power of JavaScript expressions inside all data bindings:

{{ number + 1 }}

{{ ok ? &#39;YES&#39; : &#39;NO&#39; }}

{{ message.split(&#39;&#39;).reverse().join(&#39;&#39;) }}

\&lt;div v-bind:id=&quot;&#39;list-&#39; + id&quot;\&gt;\&lt;/div\&gt;

These expressions will be evaluated as JavaScript in the data scope of the current active instance. One restriction is that each binding can only contain one single expression, so the following will NOT work:

\&lt;!-- this is a statement, not an expression: --\&gt;

{{ var a = 1 }}

\&lt;!-- flow control won&#39;t work either, use ternary expressions --\&gt;

{{ if (ok) { return message }}}

## [#](https://v3.vuejs.org/guide/template-syntax.html#directives)Directives

Directives are special attributes with the v- prefix. Directive attribute values are expected to be a single JavaScript expression (with the exception of v-for and v-on, which will be discussed later). A directive&#39;s job is to reactively apply side effects to the DOM when the value of its expression changes. Let&#39;s review the example we saw in the introduction:

\&lt;p v-if=&quot;seen&quot;\&gt;Now you see me\&lt;/p\&gt;

Here, the v-if directive would remove/insert the \&lt;p\&gt; element based on the truthiness of the value of the expression seen.

### [#](https://v3.vuejs.org/guide/template-syntax.html#arguments)Arguments

Some directives can take an &quot;argument&quot;, denoted by a colon after the directive name. For example, the v-bind directive is used to reactively update an HTML attribute:

\&lt;a v-bind:href=&quot;url&quot;\&gt; ... \&lt;/a\&gt;

Here href is the argument, which tells the v-bind directive to bind the element&#39;s href attribute to the value of the expression url.

Another example is the v-on directive, which listens to DOM events:

\&lt;a v-on:click=&quot;doSomething&quot;\&gt; ... \&lt;/a\&gt;

Here the argument is the event name to listen to. We will talk about event handling in more detail too.

### [#](https://v3.vuejs.org/guide/template-syntax.html#dynamic-arguments)Dynamic Arguments

It is also possible to use a JavaScript expression in a directive argument by wrapping it with square brackets:

\&lt;!--

Note that there are some constraints to the argument expression, as explained

in the &quot;Dynamic Argument Expression Constraints&quot; section below.

--\&gt;

\&lt;a v-bind:[attributeName]=&quot;url&quot;\&gt; ... \&lt;/a\&gt;

Here attributeName will be dynamically evaluated as a JavaScript expression, and its evaluated value will be used as the final value for the argument. For example, if your component instance has a data property, attributeName, whose value is &quot;href&quot;, then this binding will be equivalent to v-bind:href.

Similarly, you can use dynamic arguments to bind a handler to a dynamic event name:

\&lt;a v-on:[eventName]=&quot;doSomething&quot;\&gt; ... \&lt;/a\&gt;

In this example, when eventName&#39;s value is &quot;focus&quot;, v-on:[eventName] will be equivalent to v-on:focus.

### [#](https://v3.vuejs.org/guide/template-syntax.html#modifiers)Modifiers

Modifiers are special postfixes denoted by a dot, which indicate that a directive should be bound in some special way. For example, the .prevent modifier tells the v-on directive to call event.preventDefault() on the triggered event:

\&lt;form v-on:submit.prevent=&quot;onSubmit&quot;\&gt;...\&lt;/form\&gt;

You&#39;ll see other examples of modifiers later, [for](https://v3.vuejs.org/guide/events.html#event-modifiers)[v-on](https://v3.vuejs.org/guide/events.html#event-modifiers) and [for](https://v3.vuejs.org/guide/forms.html#modifiers)[v-model](https://v3.vuejs.org/guide/forms.html#modifiers), when we explore those features.

## [#](https://v3.vuejs.org/guide/template-syntax.html#shorthands)Shorthands

The v- prefix serves as a visual cue for identifying Vue-specific attributes in your templates. This is useful when you are using Vue.js to apply dynamic behavior to some existing markup, but can feel verbose for some frequently used directives. At the same time, the need for the v- prefix becomes less important when you are building a [SPA](https://en.wikipedia.org/wiki/Single-page_application), where Vue manages every template. Therefore, Vue provides special shorthands for two of the most often used directives, v-bind and v-on:

[#](https://v3.vuejs.org/guide/template-syntax.html#v-bind-shorthand)v-bind

\&lt;!-- full syntax --\&gt;

\&lt;a v-bind:href=&quot;url&quot;\&gt; ... \&lt;/a\&gt;

\&lt;!-- shorthand --\&gt;

\&lt;a :href=&quot;url&quot;\&gt; ... \&lt;/a\&gt;

\&lt;!-- shorthand with dynamic argument --\&gt;

\&lt;a :[key]=&quot;url&quot;\&gt; ... \&lt;/a\&gt;

[#](https://v3.vuejs.org/guide/template-syntax.html#v-on-shorthand)v-on Shorthand

\&lt;!-- full syntax --\&gt;

\&lt;a v-on:click=&quot;doSomething&quot;\&gt; ... \&lt;/a\&gt;

\&lt;!-- shorthand --\&gt;

\&lt;a @click=&quot;doSomething&quot;\&gt; ... \&lt;/a\&gt;

\&lt;!-- shorthand with dynamic argument --\&gt;

\&lt;a @[event]=&quot;doSomething&quot;\&gt; ... \&lt;/a\&gt;

They may look a bit different from normal HTML, but : and @ are valid characters for attribute names and all Vue-supported browsers can parse it correctly. In addition, they do not appear in the final rendered markup. The shorthand syntax is totally optional, but you will likely appreciate it when you learn more about its usage later.

### [#](https://v3.vuejs.org/guide/template-syntax.html#caveats)Caveats

#### [#](https://v3.vuejs.org/guide/template-syntax.html#dynamic-argument-value-constraints)Dynamic Argument Value Constraints

Dynamic arguments are expected to evaluate to a string, with the exception of null. The special value null can be used to explicitly remove the binding. Any other non-string value will trigger a warning.

#### [#](https://v3.vuejs.org/guide/template-syntax.html#dynamic-argument-expression-constraints)Dynamic Argument Expression Constraints

Dynamic argument expressions have some syntax constraints because certain characters, such as spaces and quotes, are invalid inside HTML attribute names. For example, the following is invalid:

\&lt;!-- This will trigger a compiler warning. --\&gt;

\&lt;a v-bind:[&#39;foo&#39; + bar]=&quot;value&quot;\&gt; ... \&lt;/a\&gt;

We recommend replacing any complex expressions with a [computed property](https://v3.vuejs.org/guide/computed.html), one of the most fundamental pieces of Vue, which we&#39;ll cover shortly.

When using in-DOM templates (templates directly written in an HTML file), you should also avoid naming keys with uppercase characters, as browsers will coerce attribute names into lowercase:

\&lt;!--

This will be converted to v-bind:[someattr] in in-DOM templates.

Unless you have a &quot;someattr&quot; property in your instance, your code won&#39;t work.

--\&gt;

\&lt;a v-bind:[someAttr]=&quot;value&quot;\&gt; ... \&lt;/a\&gt;

Template expressions are sandboxed and only have access to a [whitelist of globals](https://github.com/vuejs/vue-next/blob/master/packages/shared/src/globalsWhitelist.ts#L3)

such as Math and Date. You should not attempt to access user defined globals in template expressions.

# Data Properties and Methods

## [#](https://v3.vuejs.org/guide/data-methods.html#data-properties)Data Properties

The data option for a component is a function. Vue calls this function as part of creating a new component instance. It should return an object, which Vue will then wrap in its reactivity system and store on the component instance as $data. For convenience, any top-level properties of that object are also exposed directly via the component instance:

const app = Vue.createApp({

data(){

return{ count:4}

}

})

const vm = app.mount(&#39;#app&#39;)

console.log(vm.$data.count)// =\&gt; 4

console.log(vm.count)// =\&gt; 4

// Assigning a value to vm.count will also update $data.count

vm.count =5

console.log(vm.$data.count)// =\&gt; 5

// ... and vice-versa

vm.$data.count =6

console.log(vm.count)// =\&gt; 6

These instance properties are only added when the instance is first created, so you need to ensure they are all present in the object returned by the data function. Where necessary, use null, undefined or some other placeholder value for properties where the desired value isn&#39;t yet available.

It is possible to add a new property directly to the component instance without including it in data. However, because this property isn&#39;t backed by the reactive $data object, it won&#39;t automatically be tracked by [Vue&#39;s reactivity system](https://v3.vuejs.org/guide/reactivity.html).

Vue uses a $ prefix when exposing its own built-in APIs via the component instance. It also reserves the prefix \_ for internal properties. You should avoid using names for top-level data properties that start with either of these characters.

## [#](https://v3.vuejs.org/guide/data-methods.html#methods)Methods

To add methods to a component instance we use the methods option. This should be an object containing the desired methods:

const app = Vue.createApp({

data() {

return { count: 4 }

},

methods: {

increment() {

// `this` will refer to the component instance

this.count++

}

}

})

const vm = app.mount(&#39;#app&#39;)

console.log(vm.count) // =\&gt; 4

vm.increment()

console.log(vm.count) // =\&gt; 5

Vue automatically binds the this value for methods so that it always refers to the component instance. This ensures that a method retains the correct this value if it&#39;s used as an event listener or callback. You should avoid using arrow functions when defining methods, as that prevents Vue from binding the appropriate this value.

Just like all other properties of the component instance, the methods are accessible from within the component&#39;s template. Inside a template they are most commonly used as event listeners:

\&lt;button @click=&quot;increment&quot;\&gt;Up vote\&lt;/button\&gt;

In the example above, the method increment will be called when the \&lt;button\&gt; is clicked.

It is also possible to call a method directly from a template. As we&#39;ll see shortly, it&#39;s usually better to use a [computed property](https://v3.vuejs.org/guide/computed.html) instead. However, using a method can be useful in scenarios where computed properties aren&#39;t a viable option. You can call a method anywhere that a template supports JavaScript expressions:

\&lt;span :title=&quot;toTitleDate(date)&quot;\&gt;

{{ formatDate(date) }}

\&lt;/span\&gt;

If the methods toTitleDate or formatDate access any reactive data then it will be tracked as a rendering dependency, just as if it had been used in the template directly.

Methods called from a template should not have any side effects, such as changing data or triggering asynchronous processes. If you find yourself tempted to do that you should probably use a [lifecycle hook](https://v3.vuejs.org/guide/instance.html#lifecycle-hooks) instead.

[#](https://v3.vuejs.org/guide/data-methods.html#debouncing-and-throttling)Debouncing and Throttling

Vue doesn&#39;t include built-in support for debouncing or throttling but it can be implemented using libraries such as [Lodash](https://lodash.com/).

In cases where a component is only used once, the debouncing can be applied directly within methods:

\&lt;script src=&quot;https://unpkg.com/lodash@4.17.20/lodash.min.js&quot;\&gt;\&lt;/script\&gt;

\&lt;script\&gt;

Vue.createApp({

methods: {

// Debouncing with Lodash

click: \_.debounce(function() {

// ... respond to click ...

}, 500)

}

}).mount(&#39;#app&#39;)

\&lt;/script\&gt;

However, this approach is potentially problematic for components that are reused because they&#39;ll all share the same debounced function. To keep the component instances independent from each other, we can add the debounced function in the created lifecycle hook:

app.component(&#39;save-button&#39;, {

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

// ... respond to click ...

}

},

template: `

\&lt;button @click=&quot;debouncedClick&quot;\&gt;

Save

\&lt;/button\&gt;

`

})

# Computed Properties and Watchers

## [#](https://v3.vuejs.org/guide/computed.html#computed-properties)Computed Properties

In-template expressions are very convenient, but they are meant for simple operations. Putting too much logic in your templates can make them bloated and hard to maintain. For example, if we have an object with a nested array:

Vue.createApp({

data(){

return{

author:{

name:&#39;John Doe&#39;,

books:[

&#39;Vue 2 - Advanced Guide&#39;,

&#39;Vue 3 - Basic Guide&#39;,

&#39;Vue 4 - The Mystery&#39;

]

}

}

}

})

And we want to display different messages depending on if author already has some books or not

\&lt;div id=&quot;computed-basics&quot;\&gt;

\&lt;p\&gt;Has published books:\&lt;/p\&gt;

\&lt;span\&gt;{{ author.books.length \&gt; 0 ? &#39;Yes&#39; : &#39;No&#39; }}\&lt;/span\&gt;

\&lt;/div\&gt;

At this point, the template is no longer simple and declarative. You have to look at it for a second before realizing that it performs a calculation depending on author.books. The problem is made worse when you want to include this calculation in your template more than once.

That&#39;s why for complex logic that includes reactive data, you should use a computed property.

### [#](https://v3.vuejs.org/guide/computed.html#basic-example)Basic Example

\&lt;div id=&quot;computed-basics&quot;\&gt;

\&lt;p\&gt;Has published books:\&lt;/p\&gt;

\&lt;span\&gt;{{ publishedBooksMessage }}\&lt;/span\&gt;

\&lt;/div\&gt;

Vue.createApp({

data(){

return{

author:{

name:&#39;John Doe&#39;,

books:[

&#39;Vue 2 - Advanced Guide&#39;,

&#39;Vue 3 - Basic Guide&#39;,

&#39;Vue 4 - The Mystery&#39;

]

}

}

},

computed:{

// a computed getter

publishedBooksMessage(){

// `this` points to the vm instance

returnthis.author.books.length \&gt;0?&#39;Yes&#39;:&#39;No&#39;

}

}

}).mount(&#39;#computed-basics&#39;)

Result:

Here we have declared a computed property publishedBooksMessage.

Try to change the value of books array in the application data and you will see how publishedBooksMessage is changing accordingly.

You can data-bind to computed properties in templates just like a normal property. Vue is aware that vm.publishedBooksMessage depends on vm.author.books, so it will update any bindings that depend on vm.publishedBooksMessage when vm.author.books changes. And the best part is that we&#39;ve created this dependency relationship declaratively: the computed getter function has no side effects, which makes it easier to test and understand.

### [#](https://v3.vuejs.org/guide/computed.html#computed-caching-vs-methods)Computed Caching vs Methods

You may have noticed we can achieve the same result by invoking a method in the expression:

\&lt;p\&gt;{{ calculateBooksMessage() }}\&lt;/p\&gt;

// in component

methods:{

calculateBooksMessage(){

returnthis.author.books.length \&gt;0?&#39;Yes&#39;:&#39;No&#39;

}

}

Instead of a computed property, we can define the same function as a method. For the end result, the two approaches are indeed exactly the same. However, the difference is that computed properties are cached based on their reactive dependencies. A computed property will only re-evaluate when some of its reactive dependencies have changed. This means as long as author.books has not changed, multiple access to the publishedBooksMessage computed property will immediately return the previously computed result without having to run the function again.

This also means the following computed property will never update, because Date.now() is not a reactive dependency:

computed:{

now(){

return Date.now()

}

}

In comparison, a method invocation will always run the function whenever a re-render happens.

Why do we need caching? Imagine we have an expensive computed property list, which requires looping through a huge array and doing a lot of computations. Then we may have other computed properties that in turn depend on list. Without caching, we would be executing list&#39;s getter many more times than necessary! In cases where you do not want caching, use a method instead.

### [#](https://v3.vuejs.org/guide/computed.html#computed-setter)Computed Setter

Computed properties are by default getter-only, but you can also provide a setter when you need it:

// ...

computed:{

fullName:{

// getter

get(){

returnthis.firstName +&#39; &#39;+this.lastName

},

// setter

set(newValue){

const names = newValue.split(&#39; &#39;)

this.firstName = names[0]

this.lastName = names[names.length -1]

}

}

}

// ...

Now when you run vm.fullName = &#39;John Doe&#39;, the setter will be invoked and vm.firstName and vm.lastName will be updated accordingly.

## [#](https://v3.vuejs.org/guide/computed.html#watchers)Watchers

While computed properties are more appropriate in most cases, there are times when a custom watcher is necessary. That&#39;s why Vue provides a more generic way to react to data changes through the watch option. This is most useful when you want to perform asynchronous or expensive operations in response to changing data.

For example:

\&lt;div id=&quot;watch-example&quot;\&gt;

\&lt;p\&gt;

Ask a yes/no question:

\&lt;input v-model=&quot;question&quot;/\&gt;

\&lt;/p\&gt;

\&lt;p\&gt;{{ answer }}\&lt;/p\&gt;

\&lt;/div\&gt;

\&lt;!-- Since there is already a rich ecosystem of ajax libraries --\&gt;

\&lt;!-- and collections of general-purpose utility methods, Vue core --\&gt;

\&lt;!-- is able to remain small by not reinventing them. This also --\&gt;

\&lt;!-- gives you the freedom to use what you&#39;re familiar with. --\&gt;

\&lt;script src=&quot;https://cdn.jsdelivr.net/npm/axios@0.12.0/dist/axios.min.js&quot;\&gt;\&lt;/script\&gt;

\&lt;script\&gt;

const watchExampleVM = Vue.createApp({

data(){

return{

question:&#39;&#39;,

answer:&#39;Questions usually contain a question mark. ;-)&#39;

}

},

watch:{

// whenever question changes, this function will run

question(newQuestion, oldQuestion){

if(newQuestion.indexOf(&#39;?&#39;)\&gt;-1){

this.getAnswer()

}

}

},

methods:{

getAnswer(){

this.answer =&#39;Thinking...&#39;

axios

.get(&#39;https://yesno.wtf/api&#39;)

.then(response =\&gt;{

this.answer = response.data.answer

})

.catch(error =\&gt;{

this.answer =&#39;Error! Could not reach the API. &#39;+ error

})

}

}

}).mount(&#39;#watch-example&#39;)

\&lt;/script\&gt;

Result:

In this case, using the watch option allows us to perform an asynchronous operation (accessing an API) and sets a condition for performing this operation. None of that would be possible with a computed property.

In addition to the watch option, you can also use the imperative [vm.$watch API](https://v3.vuejs.org/api/instance-methods.html#watch).

### [#](https://v3.vuejs.org/guide/computed.html#computed-vs-watched-property)Computed vs Watched Property

Vue does provide a more generic way to observe and react to data changes on a current active instance: watch properties. When you have some data that needs to change based on some other data, it is tempting to overuse watch - especially if you are coming from an AngularJS background. However, it is often a better idea to use a computed property rather than an imperative watch callback. Consider this example:

\&lt;div id=&quot;demo&quot;\&gt;{{ fullName }}\&lt;/div\&gt;

const vm = Vue.createApp({

data(){

return{

firstName:&#39;Foo&#39;,

lastName:&#39;Bar&#39;,

fullName:&#39;Foo Bar&#39;

}

},

watch:{

firstName(val){

this.fullName = val +&#39; &#39;+this.lastName

},

lastName(val){

this.fullName =this.firstName +&#39; &#39;+ val

}

}

}).mount(&#39;#demo&#39;)

The above code is imperative and repetitive. Compare it with a computed property version:

const vm = Vue.createApp({

data(){

return{

firstName:&#39;Foo&#39;,

lastName:&#39;Bar&#39;

}

},

computed:{

fullName(){

returnthis.firstName +&#39; &#39;+this.lastName

}

}

}).mount(&#39;#demo&#39;)

Much better, isn&#39;t it?

# Class and Style Bindings

A common need for data binding is manipulating an element&#39;s class list and its inline styles. Since they are both attributes, we can use v-bind to handle them: we only need to calculate a final string with our expressions. However, meddling with string concatenation is annoying and error-prone. For this reason, Vue provides special enhancements when v-bind is used with class and style. In addition to strings, the expressions can also evaluate to objects or arrays.

## [#](https://v3.vuejs.org/guide/class-and-style.html#binding-html-classes)Binding HTML Classes

### [#](https://v3.vuejs.org/guide/class-and-style.html#object-syntax)Object Syntax

We can pass an object to :class (short for v-bind:class) to dynamically toggle classes:

\&lt;div :class=&quot;{ active: isActive }&quot;\&gt;\&lt;/div\&gt;

The above syntax means the presence of the active class will be determined by the [truthiness](https://developer.mozilla.org/en-US/docs/Glossary/Truthy)

[(opens new window)](https://developer.mozilla.org/en-US/docs/Glossary/Truthy)

of the data property isActive.

You can have multiple classes toggled by having more fields in the object. In addition, the :class directive can also co-exist with the plain class attribute. So given the following template:

\&lt;div

class=&quot;static&quot;

:class=&quot;{ active: isActive, &#39;text-danger&#39;: hasError }&quot;

\&gt;\&lt;/div\&gt;

And the following data:

data(){

return{

isActive:true,

hasError:false

}

}

It will render:

\&lt;div class=&quot;static active&quot;\&gt;\&lt;/div\&gt;

When isActive or hasError changes, the class list will be updated accordingly. For example, if hasError becomes true, the class list will become &quot;static active text-danger&quot;.

The bound object doesn&#39;t have to be inline:

\&lt;div :class=&quot;classObject&quot;\&gt;\&lt;/div\&gt;

data(){

return{

classObject:{

active:true,

&#39;text-danger&#39;:false

}

}

}

This will render the same result. We can also bind to a [computed property](https://v3.vuejs.org/guide/computed.html) that returns an object. This is a common and powerful pattern:

\&lt;div :class=&quot;classObject&quot;\&gt;\&lt;/div\&gt;

data(){

return{

isActive:true,

error:null

}

},

computed:{

classObject(){

return{

active:this.isActive &amp;&amp;!this.error,

&#39;text-danger&#39;:this.error &amp;&amp;this.error.type ===&#39;fatal&#39;

}

}

}

### [#](https://v3.vuejs.org/guide/class-and-style.html#array-syntax)Array Syntax

We can pass an array to :class to apply a list of classes:

\&lt;div :class=&quot;[activeClass, errorClass]&quot;\&gt;\&lt;/div\&gt;

data(){

return{

activeClass:&#39;active&#39;,

errorClass:&#39;text-danger&#39;

}

}

Which will render:

\&lt;div class=&quot;active text-danger&quot;\&gt;\&lt;/div\&gt;

If you would like to also toggle a class in the list conditionally, you can do it with a ternary expression:

\&lt;div :class=&quot;[isActive ? activeClass : &#39;&#39;, errorClass]&quot;\&gt;\&lt;/div\&gt;

This will always apply errorClass, but activeClass will only be applied when isActive is truthy.

However, this can be a bit verbose if you have multiple conditional classes. That&#39;s why it&#39;s also possible to use the object syntax inside array syntax:

\&lt;div :class=&quot;[{ active: isActive }, errorClass]&quot;\&gt;\&lt;/div\&gt;

### [#](https://v3.vuejs.org/guide/class-and-style.html#with-components)With Components

When you use the class attribute on a custom component with a single root element, those classes will be added to this element. Existing classes on this element will not be overwritten.

For example, if you declare this component:

const app = Vue.createApp({})

app.component(&#39;my-component&#39;,{

template:`\&lt;p class=&quot;foo bar&quot;\&gt;Hi!\&lt;/p\&gt;`

})

Then add some classes when using it:

\&lt;div id=&quot;app&quot;\&gt;

\&lt;my-component class=&quot;baz boo&quot;\&gt;\&lt;/my-component\&gt;

\&lt;/div\&gt;

The rendered HTML will be:

\&lt;p class=&quot;foo bar baz boo&quot;\&gt;Hi\&lt;/p\&gt;

The same is true for class bindings:

\&lt;my-component :class=&quot;{ active: isActive }&quot;\&gt;\&lt;/my-component\&gt;

When isActive is truthy, the rendered HTML will be:

\&lt;p class=&quot;foo bar active&quot;\&gt;Hi\&lt;/p\&gt;

If your component has multiple root elements, you would need to define which component will receive this class. You can do this using $attrs component property:

\&lt;div id=&quot;app&quot;\&gt;

\&lt;my-component class=&quot;baz&quot;\&gt;\&lt;/my-component\&gt;

\&lt;/div\&gt;

const app = Vue.createApp({})

app.component(&#39;my-component&#39;,{

template:`

\&lt;p :class=&quot;$attrs.class&quot;\&gt;Hi!\&lt;/p\&gt;

\&lt;span\&gt;This is a child component\&lt;/span\&gt;

`

})

You can learn more about component attribute inheritance in the Non-Prop[Attributes](https://v3.vuejs.org/guide/component-attrs.html) section.

## [#](https://v3.vuejs.org/guide/class-and-style.html#binding-inline-styles)Binding Inline Styles

### [#](https://v3.vuejs.org/guide/class-and-style.html#object-syntax-2)Object Syntax

The object syntax for :style is pretty straightforward - it looks almost like CSS, except it&#39;s a JavaScript object. You can use either camelCase or kebab-case (use quotes with kebab-case) for the CSS property names:

\&lt;div :style=&quot;{color: activeColor,fontSize: fontSize + &#39;px&#39; }&quot;\&gt;\&lt;/div\&gt;

data(){

return{

activeColor:&#39;red&#39;,

fontSize:30

}

}

It is often a good idea to bind to a style object directly so that the template is cleaner:

\&lt;div :style=&quot;styleObject&quot;\&gt;\&lt;/div\&gt;

data(){

return{

styleObject:{

color:&#39;red&#39;,

fontSize:&#39;13px&#39;

}

}

}

Again, the object syntax is often used in conjunction with computed properties that return objects.

### [#](https://v3.vuejs.org/guide/class-and-style.html#array-syntax-2)Array Syntax

The array syntax for :style allows you to apply multiple style objects to the same element:

\&lt;div :style=&quot;[baseStyles, overridingStyles]&quot;\&gt;\&lt;/div\&gt;

### [#](https://v3.vuejs.org/guide/class-and-style.html#auto-prefixing)Auto-prefixing

When you use a CSS property that requires [vendor prefixes](https://developer.mozilla.org/en-US/docs/Glossary/Vendor_Prefix)

in :style, for example transform, Vue will automatically detect and add appropriate prefixes to the applied styles.

### [#](https://v3.vuejs.org/guide/class-and-style.html#multiple-values)Multiple Values

You can provide an array of multiple (prefixed) values to a style property, for example:

\&lt;div :style=&quot;{display: [&#39;-webkit-box&#39;, &#39;-ms-flexbox&#39;, &#39;flex&#39;] }&quot;\&gt;\&lt;/div\&gt;

This will only render the last value in the array which the browser supports. In this example, it will render display: flex for browsers that support the unprefixed version of flexbox.

# Conditional Rendering

## [#](https://v3.vuejs.org/guide/conditional.html#v-if)v-if

The directive v-if is used to conditionally render a block. The block will only be rendered if the directive&#39;s expression returns a truthy value.

\&lt;h1 v-if=&quot;awesome&quot;\&gt;Vue is awesome!\&lt;/h1\&gt;

It is also possible to add an &quot;else block&quot; with v-else:

\&lt;h1 v-if=&quot;awesome&quot;\&gt;Vue is awesome!\&lt;/h1\&gt;

\&lt;h1 v-else\&gt;Oh no 😢\&lt;/h1\&gt;

### [#](https://v3.vuejs.org/guide/conditional.html#conditional-groups-with-v-if-on-template)Conditional Groups with v-if on \&lt;template\&gt;

Because v-if is a directive, it has to be attached to a single element. But what if we want to toggle more than one element? In this case we can use v-if on a \&lt;template\&gt; element, which serves as an invisible wrapper. The final rendered result will not include the \&lt;template\&gt; element.

\&lt;template v-if=&quot;ok&quot;\&gt;

\&lt;h1\&gt;Title\&lt;/h1\&gt;

\&lt;p\&gt;Paragraph 1\&lt;/p\&gt;

\&lt;p\&gt;Paragraph 2\&lt;/p\&gt;

\&lt;/template\&gt;

### [#](https://v3.vuejs.org/guide/conditional.html#v-else)v-else

You can use the v-else directive to indicate an &quot;else block&quot; for v-if:

\&lt;div v-if=&quot;Math.random() \&gt; 0.5&quot;\&gt;

Now you see me

\&lt;/div\&gt;

\&lt;div v-else\&gt;

Now you don&#39;t

\&lt;/div\&gt;

A v-else element must immediately follow a v-if or a v-else-if element - otherwise it will not be recognized.

### [#](https://v3.vuejs.org/guide/conditional.html#v-else-if)v-else-if

The v-else-if, as the name suggests, serves as an &quot;else if block&quot; for v-if. It can also be chained multiple times:

\&lt;div v-if=&quot;type === &#39;A&#39;&quot;\&gt;

A

\&lt;/div\&gt;

\&lt;div v-else-if=&quot;type === &#39;B&#39;&quot;\&gt;

B

\&lt;/div\&gt;

\&lt;div v-else-if=&quot;type === &#39;C&#39;&quot;\&gt;

C

\&lt;/div\&gt;

\&lt;div v-else\&gt;

Not A/B/C

\&lt;/div\&gt;

Similar to v-else, a v-else-if element must immediately follow a v-if or a v-else-if element.

## [#](https://v3.vuejs.org/guide/conditional.html#v-show)v-show

Another option for conditionally displaying an element is the v-show directive. The usage is largely the same:

\&lt;h1 v-show=&quot;ok&quot;\&gt;Hello!\&lt;/h1\&gt;

The difference is that an element with v-show will always be rendered and remain in the DOM; v-show only toggles the display CSS property of the element.

v-show doesn&#39;t support the \&lt;template\&gt; element, nor does it work with v-else.

## [#](https://v3.vuejs.org/guide/conditional.html#v-if-vs-v-show)v-if vs v-show

v-if is &quot;real&quot; conditional rendering because it ensures that event listeners and child components inside the conditional block are properly destroyed and re-created during toggles.

v-if is also lazy: if the condition is false on initial render, it will not do anything - the conditional block won&#39;t be rendered until the condition becomes true for the first time.

In comparison, v-show is much simpler - the element is always rendered regardless of initial condition, with CSS-based toggling.

Generally speaking, v-if has higher toggle costs while v-show has higher initial render costs. So prefer v-show if you need to toggle something very often, and prefer v-if if the condition is unlikely to change at runtime.

## [#](https://v3.vuejs.org/guide/conditional.html#v-if-with-v-for)v-if with v-for

Note

Using v-if and v-for together is not recommended. See the [style guide](https://v3.vuejs.org/style-guide/#avoid-v-if-with-v-for-essential) for further information.

When v-if and v-for are both used on the same element, v-if will be evaluated first. See the [list rendering guide](https://v3.vuejs.org/guide/list#v-for-with-v-if) for details.

# List Rendering

## [#](https://v3.vuejs.org/guide/list.html#mapping-an-array-to-elements-with-v-for)Mapping an Array to Elements with v-for

We can use the v-for directive to render a list of items based on an array. The v-for directive requires a special syntax in the form of item in items, where items is the source data array and item is an alias for the array element being iterated on:

\&lt;ul id=&quot;array-rendering&quot;\&gt;

\&lt;li v-for=&quot;item in items&quot;\&gt;

{{ item.message }}

\&lt;/li\&gt;

\&lt;/ul\&gt;

Vue.createApp({

data(){

return{

items:[{ message:&#39;Foo&#39;},{ message:&#39;Bar&#39;}]

}

}

}).mount(&#39;#array-rendering&#39;)

Result:

Inside v-for blocks we have full access to parent scope properties. v-for also supports an optional second argument for the index of the current item.

\&lt;ul id=&quot;array-with-index&quot;\&gt;

\&lt;li v-for=&quot;(item, index) in items&quot;\&gt;

{{ parentMessage }} - {{ index }} - {{ item.message }}

\&lt;/li\&gt;

\&lt;/ul\&gt;

Vue.createApp({

data(){

return{

parentMessage:&#39;Parent&#39;,

items:[{ message:&#39;Foo&#39;},{ message:&#39;Bar&#39;}]

}

}

}).mount(&#39;#array-with-index&#39;)

Result:

You can also use of as the delimiter instead of in, so that it is closer to JavaScript&#39;s syntax for iterators:

\&lt;div v-for=&quot;item of items&quot;\&gt;\&lt;/div\&gt;

## [#](https://v3.vuejs.org/guide/list.html#v-for-with-an-object)v-for with an Object

You can also use v-for to iterate through the properties of an object.

\&lt;ul id=&quot;v-for-object&quot; class=&quot;demo&quot;\&gt;

\&lt;li v-for=&quot;value in myObject&quot;\&gt;

{{ value }}

\&lt;/li\&gt;

\&lt;/ul\&gt;

Vue.createApp({

data(){

return{

myObject:{

title:&#39;How to do lists in Vue&#39;,

author:&#39;Jane Doe&#39;,

publishedAt:&#39;2016-04-10&#39;

}

}

}

}).mount(&#39;#v-for-object&#39;)

Result:

You can also provide a second argument for the property&#39;s name (a.k.a. key):

\&lt;li v-for=&quot;(value, name) in myObject&quot;\&gt;

{{ name }}: {{ value }}

\&lt;/li\&gt;

And another for the index:

\&lt;li v-for=&quot;(value, name, index) in myObject&quot;\&gt;

{{ index }}. {{ name }}: {{ value }}

\&lt;/li\&gt;

Note

When iterating over an object, the order is based on the enumeration order of Object.keys(), which isn&#39;t guaranteed to be consistent across JavaScript engine implementations.

## [#](https://v3.vuejs.org/guide/list.html#maintaining-state)Maintaining State

When Vue is updating a list of elements rendered with v-for, by default it uses an &quot;in-place patch&quot; strategy. If the order of the data items has changed, instead of moving the DOM elements to match the order of the items, Vue will patch each element in-place and make sure it reflects what should be rendered at that particular index.

This default mode is efficient, but only suitable when your list render output does not rely on child component state or temporary DOM state (e.g. form input values).

To give Vue a hint so that it can track each node&#39;s identity, and thus reuse and reorder existing elements, you need to provide a unique key attribute for each item:

\&lt;div v-for=&quot;item in items&quot; :key=&quot;item.id&quot;\&gt;

\&lt;!-- content --\&gt;

\&lt;/div\&gt;

It is recommended to provide a key attribute with v-for whenever possible, unless the iterated DOM content is simple, or you are intentionally relying on the default behavior for performance gains.

Since it&#39;s a generic mechanism for Vue to identify nodes, the key also has other uses that are not specifically tied to v-for, as we will see later in the guide.

Note

Don&#39;t use non-primitive values like objects and arrays as v-for keys. Use string or numeric values instead.

For detailed usage of the key attribute, please see the [key](https://v3.vuejs.org/api/special-attributes.html#key)[API documentation](https://v3.vuejs.org/api/special-attributes.html#key).

## [#](https://v3.vuejs.org/guide/list.html#array-change-detection)Array Change Detection

### [#](https://v3.vuejs.org/guide/list.html#mutation-methods)Mutation Methods

Vue wraps an observed array&#39;s mutation methods so they will also trigger view updates. The wrapped methods are:

- push()
- pop()
- shift()
- unshift()
- splice()
- sort()
- reverse()

You can open the console and play with the previous examples&#39; items array by calling their mutation methods. For example: example1.items.push({ message: &#39;Baz&#39; }).

### [#](https://v3.vuejs.org/guide/list.html#replacing-an-array)Replacing an Array

Mutation methods, as the name suggests, mutate the original array they are called on. In comparison, there are also non-mutating methods, e.g. filter(), concat() and slice(), which do not mutate the original array but always return a new array. When working with non-mutating methods, you can replace the old array with the new one:

example1.items = example1.items.filter(item =\&gt; item.message.match(/Foo/))1

You might think this will cause Vue to throw away the existing DOM and re-render the entire list - luckily, that is not the case. Vue implements some smart heuristics to maximize DOM element reuse, so replacing an array with another array containing overlapping objects is a very efficient operation.

## [#](https://v3.vuejs.org/guide/list.html#displaying-filtered-sorted-results)Displaying Filtered/Sorted Results

Sometimes we want to display a filtered or sorted version of an array without actually mutating or resetting the original data. In this case, you can create a computed property that returns the filtered or sorted array.

For example:

\&lt;li v-for=&quot;n in evenNumbers&quot; :key=&quot;n&quot;\&gt;{{ n }}\&lt;/li\&gt;

data(){

return{

numbers:[1,2,3,4,5]

}

},

computed:{

evenNumbers(){

returnthis.numbers.filter(number =\&gt; number %2===0)

}

}

In situations where computed properties are not feasible (e.g. inside nested v-for loops), you can use a method:

\&lt;ul v-for=&quot;numbers in sets&quot;\&gt;

\&lt;li v-for=&quot;n in even(numbers)&quot; :key=&quot;n&quot;\&gt;{{ n }}\&lt;/li\&gt;

\&lt;/ul\&gt;

data(){

return{

sets:[[1,2,3,4,5],[6,7,8,9,10]]

}

},

methods:{

even(numbers){

return numbers.filter(number =\&gt; number %2===0)

}

}

## [#](https://v3.vuejs.org/guide/list.html#v-for-with-a-range)v-for with a Range

v-for can also take an integer. In this case it will repeat the template that many times.

\&lt;div id=&quot;range&quot; class=&quot;demo&quot;\&gt;

\&lt;span v-for=&quot;n in 10&quot; :key=&quot;n&quot;\&gt;{{ n }} \&lt;/span\&gt;

\&lt;/div\&gt;

Result:

## [#](https://v3.vuejs.org/guide/list.html#v-for-on-a-template)v-for on a \&lt;template\&gt;

Similar to template v-if, you can also use a \&lt;template\&gt; tag with v-for to render a block of multiple elements. For example:

\&lt;ul\&gt;

\&lt;template v-for=&quot;item in items&quot; :key=&quot;item.msg&quot;\&gt;

\&lt;li\&gt;{{ item.msg }}\&lt;/li\&gt;

\&lt;li class=&quot;divider&quot; role=&quot;presentation&quot;\&gt;\&lt;/li\&gt;

\&lt;/template\&gt;

\&lt;/ul\&gt;

## [#](https://v3.vuejs.org/guide/list.html#v-for-with-v-if)v-for with v-if

TIP

Note that it&#39;s not recommended to use v-if and v-for together. Refer to the style[guide](https://v3.vuejs.org/style-guide/#avoid-v-if-with-v-for-essential) for details.

When they exist on the same node, v-if has a higher priority than v-for. That means the v-if condition will not have access to variables from the scope of the v-for:

\&lt;!-- This will throw an error because property &quot;todo&quot; is not defined on instance. --\&gt;

\&lt;li v-for=&quot;todo in todos&quot; v-if=&quot;!todo.isComplete&quot;\&gt;

{{ todo.name }}

\&lt;/li\&gt;

This can be fixed by moving v-for to a wrapping \&lt;template\&gt; tag:

\&lt;template v-for=&quot;todo in todos&quot; :key=&quot;todo.name&quot;\&gt;

\&lt;li v-if=&quot;!todo.isComplete&quot;\&gt;

{{ todo.name }}

\&lt;/li\&gt;

\&lt;/template\&gt;

## [#](https://v3.vuejs.org/guide/list.html#v-for-with-a-component)v-for with a Component

This section assumes knowledge of [Components](https://v3.vuejs.org/guide/component-basics.html). Feel free to skip it and come back later.

You can directly use v-for on a custom component, like any normal element:

\&lt;my-component v-for=&quot;item in items&quot; :key=&quot;item.id&quot;\&gt;\&lt;/my-component\&gt;

However, this won&#39;t automatically pass any data to the component, because components have isolated scopes of their own. In order to pass the iterated data into the component, we should also use props:

\&lt;my-component

v-for=&quot;(item, index) in items&quot;

:item=&quot;item&quot;

:index=&quot;index&quot;

:key=&quot;item.id&quot;

\&gt;\&lt;/my-component\&gt;

The reason for not automatically injecting item into the component is because that makes the component tightly coupled to how v-for works. Being explicit about where its data comes from makes the component reusable in other situations.

Here&#39;s a complete example of a simple todo list:

\&lt;div id=&quot;todo-list-example&quot;\&gt;

\&lt;form v-on:submit.prevent=&quot;addNewTodo&quot;\&gt;

\&lt;label for=&quot;new-todo&quot;\&gt;Add a todo\&lt;/label\&gt;

\&lt;input

v-model=&quot;newTodoText&quot;

id=&quot;new-todo&quot;

placeholder=&quot;E.g. Feed the cat&quot;

/\&gt;

\&lt;button\&gt;Add\&lt;/button\&gt;

\&lt;/form\&gt;

\&lt;ul\&gt;

\&lt;todo-item

v-for=&quot;(todo, index) in todos&quot;

:key=&quot;todo.id&quot;

:title=&quot;todo.title&quot;

@remove=&quot;todos.splice(index, 1)&quot;

\&gt;\&lt;/todo-item\&gt;

\&lt;/ul\&gt;

\&lt;/div\&gt;

const app = Vue.createApp({

data(){

return{

newTodoText:&#39;&#39;,

todos:[

{

id:1,

title:&#39;Do the dishes&#39;

},

{

id:2,

title:&#39;Take out the trash&#39;

},

{

id:3,

title:&#39;Mow the lawn&#39;

}

],

nextTodoId:4

}

},

methods:{

addNewTodo(){

this.todos.push({

id:this.nextTodoId++,

title:this.newTodoText

})

this.newTodoText =&#39;&#39;

}

}

})

app.component(&#39;todo-item&#39;,{

template:`

\&lt;li\&gt;

{{ title }}

\&lt;button @click=&quot;$emit(&#39;remove&#39;)&quot;\&gt;Remove\&lt;/button\&gt;

\&lt;/li\&gt;

`,

props:[&#39;title&#39;],

emits:[&#39;remove&#39;]

})

app.mount(&#39;#todo-list-example&#39;)

# Main Files

## App.vue

App.vue is a Single File Component and is a great way to create self-contained components that have all they need in a single file. We have the markup, the JavaScript that is going to interact with it, and style that&#39;s applied to it, which can be scoped, or not. In this case, it&#39;s not scoped, and it&#39;s just outputting that CSS which is applied like regular CSS to the page. The interesting part lies in the script tag where all relevant components are declared as a dependency. ![](RackMultipart20210310-4-fcaz0h_html_8d432fe38af9822e.png)

When a Vue instance is created, it adds all the properties found in its data object to Vue&#39;s reactivity system. When the values of those properties change, the view will &quot;react&quot;, updating to match the new values. When \&lt;\&lt; data \&gt;\&gt; changes, the view will re-render. It should be noted that properties in data are only reactive if they existed when the instance was created.

VBUS - custom event bus for letting unrelated components talk to each other. Initialize Top bar, footer, relevant theme scss file and relevant styling class(es)

## Miniwin.vue

All key components along with agrs &amp; necessary transitions to form a Mini Window for Projects Platform. It is one the key components along with TopBar, Big Window, Application Dialog, Popup &amp; Message components to show the information and preview Project data.

## Msg.vue

Leverage UserCard for displaying messages of the passed argument with appropriate transitions.

## BigWin.vue

We can use the v-on directive to listen to DOM events and run some JavaScript when they&#39;re triggered. Detects the mode in which the Projects platform is being utilized.

## **TopBar.vue**

TopBar components with the relevant logo information (based on organizations) along with portal language, search portal button with material icons for small display sizes, online help documentation along with project category icon. Google login button redirects them to keycloak login, logout windows based on user authentication status. The TopBar is a shared component that includes organization brand collaterals (conditional logo &amp; branding), portal language (currently English, French &amp; Simplified Chinese), search (currently database search not elastic search), contextual help (end user documentation) and user&#39;s profile avatar and name(if user is logged in).

![](RackMultipart20210310-4-fcaz0h_html_d0f4517a60ada609.png)

## **Main.css**

Key CSS file for #APP and other key views stylings.

## **Main.js**

Key js consequential file where the Projects platform starts. The external libraries like JQuery, Leaflet, Bulma, Axios etc. are imported in main.js. This is where the global inter component communication bus **VBUS** is initialized along with pre-configuring Axios according to the organization id .

Computed properties let perform complex operations or data formatting while maximizing performance with dependency calculations that only update the view when a dependency changes. This feature is synchronous. However, we leverage the _vue-async-computed_ package to create and consume asynchronous computed properties in projects&#39; components by binding the resolved value of a Promise to a component property.

The **Translate** function uses Translate JSON file to make Projects platform multilingual to include multiple labels in multiple languages to be swapped on user selection. The toHtmlTB function makes addition or deletion of language(s) easy &amp; modular.

This is the file that initializes export of Global Shared Object (GS) as a substitute for state handling external libraries like Vuex. The object seeds the categories according to the organizations along with the API data properties linked to the user(people) and the organization. We use [**URLSearchParams**](https://developer.mozilla.org/en-US/docs/Web/API/URLSearchParams) to define utility methods to work with the query string of a URL. GS object implementing URLSearchParams can directly be used in a &quot;for...of&quot; structure that allows us to manipulate the state and check connection by returning the first value associated with the given search parameter and allowing iteration through all keys of the key/value pairs contained in this object. Key point to note is that URLSearchParams constructor does not parse full URLs. However, it will strip an initial leading ? off of a string, if present.

The **history**. **replaceState** () method modifies the current history entry, replacing it with the stateObj, title, and URL passed in the method parameters. This method is particularly useful when you want to update the state object or URL of the current history entry in response to some user action.

![](RackMultipart20210310-4-fcaz0h_html_d3ee22e7f82e4974.png)

We leverage AXIOS post to send bearer tokens where the first parameter is the URL. The second is the JSON body that will be sent along the request. The third parameter are the headers (among other things), which is JSON as well.

![](RackMultipart20210310-4-fcaz0h_html_5d76e8657be4643c.png)

The same helps ascertain users authorization levels and check the connection loop to initialize Projects Platform in the right state based on user&#39;s authorization &amp; authentication level. Projects Platform application uses function **initProjects** () to configure all the global Axios defaults. [Axios interceptors](https://github.com/axios/axios#interceptors) intercept requests or responses before they are handled by then or catch. The interceptors are used to append every request with XSRF tokens for security and to catch all global errors and return AMIGA guru meditation errors(What!!!) linked with 401, 403, 417, 422, 501 error codes. Key thing to note is that the request interceptors are presumed to be asynchronous by default. This can cause a delay in the execution of the axios request when the main thread is blocked (a promise is created under the hood for the interceptor and the request gets put on the bottom of the call stack). If request interceptors are synchronous we could add a flag to the options object that will tell axios to run the code synchronously and avoid any delays in request execution. The initialize function sets the current theme, portal language and relevant organization parameters including main categories, stylings.

## **Router.js**

Router file leverages Vue Router to put all the Projects platform components in hierarchy explicitly mentioning child parent relationships (route nesting). The key part to focus on in this file is that the routes of our Vue app are defined via an array that contains objects. Each route object contains three key properties:

- Path - what URL should match to the component.
- Name - what this route should be named for labeling and debugging purposes.
- Component - the component that should be displayed when the path is matched.

routes: [

{

path: &#39;/&#39;,

name: &#39;Home&#39;,

component: pageHome

},

{

path: &#39;/logout&#39;,

beforeEnter() { location.href=GS.apisrv+&#39;/logout?home=&#39;+ btoa(window.location.origin) }

},

{

path: &#39;/me&#39;,

name: &#39;myhomepage&#39;,

component: pageMe,

children: [

{ path: &#39;followed&#39;,

name: &quot;followed&quot;,

component: subMeFollowed,

},

{ path: &#39;myprojects&#39;,

name: &quot;myprojects&quot;,

component: subMeMyProjects,

},

{ path: &#39;toreview&#39;,

name: &quot;toreview&quot;,

component: subMeReviewed,

},

]

},

{

path: &#39;/admin&#39;,

name: &#39;Admin&#39;,

component: pageAdmin,

children: [

{ path: &#39;portal&#39;,

name: &quot;portal&quot;,

component: PortalAdmin,

children: [

{

path: &#39;general&#39;,

name: &quot;general&quot;,

component: PortalGeneralAdmin,

},

{

path: &#39;concepts&#39;,

name: &quot;concepts&quot;,

component: ConceptsAdmin,

},

{

path: &#39;types&#39;,

name: &quot;types&quot;,

component: TypesAdmin,

}

]

},

{ path: &#39;contents&#39;,

name: &quot;contents&quot;,

component: ContentAdmin,

},

{ path: &#39;users&#39;,

name: &quot;users&quot;,

component: UserAdmin,

}

]

},

{

path: &#39;/repo/&#39;,

name: &#39;type&#39;,

component: pageCat,

props: true

},

{

path: &#39;/repo/:type&#39;,

name: &#39;type&#39;,

component: pageCat,

props: true

},

{

path: &#39;/projects&#39;,

name: &#39;projects&#39;,

component: pageBrowse,

},

{

path: &#39;/map&#39;,

name: &#39;map&#39;,

component: pageMap,

},

{

path: &#39;/concepts-map&#39;,

name: &#39;concepts-map&#39;,

component: ConceptsMap

},

{

path: &#39;/projects/:id&#39;,

name: &#39;pageproject&#39;,

component: pageProject,

children: [

{ path: &#39;summary&#39;,

name: &quot;projectsummary&quot;,

component: subProjectSummary,

},

{ path: &#39;des&#39;,

name: &quot;projectdes&quot;,

component: subProjectDes,

},

{ path: &#39;blogentries&#39;,

name: &quot;projectblog&quot;,

component: subProjectBlog,

},

{ path: &#39;goals&#39;,

name: &quot;projectgoals&quot;,

component: subProjectGoals,

},

{ path: &#39;team&#39;,

name: &quot;projectteam&quot;,

component: subProjectTeam,

},

{ path: &#39;ressources&#39;,

name: &quot;projectressources&quot;,

component: subProjectRes,

},

{ path: &#39;comments&#39;,

name: &quot;projectcomments&quot;,

component: subProjectComments,

},

]

},

{

path: &#39;/editproject/:id&#39;,

component: pageEditProject,

children: [

{ path: &#39;general&#39;,

name: &quot;editproject&quot;,

component: subEditProjectGen,

},

]

},

{

path: &#39;/stats&#39;,

name: &quot;stat&quot;,

component: Stat

}

]

})

## **AppDialog.vue**

Parent component of Gallery &amp; Video provider chooser components that allows inclusion of Image gallery &amp; Video embed components.

## **PopUp.vue**

Parent component for Error, Info &amp; Progress components with mode &amp; arguments as props with relevant transitions.

# Shared Components

### Admin Sidebar

#### Admin Routes (js)

#### Admin Sidebar (vue)

#### Menu Item (vue)

# Functions

### API

### Organizations Services (js)

Specific file for retrieving &amp; updating leveraging AXIOS Get &amp; Patch operations. The filter for fetching organisations according to concepts and using getAxiosConfig with etag token for updating respective organizations passing the formData as an argument from the Portal general Admin component.

### Types Services (js)

Specialized file for projects&#39; types that helps projects platform users thematically differentiate the projects. There CRUD operations around the project types that are synchronous(mainly get(getType) and filter operations by respective organizations(getTypesByOrg)) or asynchronous leveraging Axios post(addType), patch(updateType), delete(deleteType).

### API services (js)

Central definition for all the relevant functions that are utilized across the Projects platform code including Image upload, file upload, search in PeopleAPI, get specific user, wiki concepts (category) &amp; project, publish projects, project CRUD dispositions, project categories, blog entries, SDGs, 3rd party resources, project reviews &amp; comments, organization(s) and make GET, POST, PATCH, DELETE request(s) using Axios to get, push, patch, post and delete data to/from a given endpoint and trigger events.

Imports Global shared(GS) object and utilizes a 3rd party library like Axios that is an HTTP client library which uses promises by default and runs on both the client and the server, which makes it appropriate for fetching data during server-side rendering. Because it uses promises, we combine it with async/await to get a concise and easy-to-use API.

### Constants (js)

Declare constants in a separate constants.js file which we can require into the other Vue component:

- Sustainable Development Goals(SDG) Codes
- SDG labels
- SDG Colors
- Months
- Media file Upload Constraints

### Dotatlas (js)

dotAtlas is a JavaScript library for interactive exploration of 2d point collections. dotAtlas can produce zoomable visualizations similar to the one shown below. They combine various types of layers, such as elevations, markers or labels, to produce an attractive map-like presentation of your data.

![](RackMultipart20210310-4-fcaz0h_html_d04864ca03764aa3.jpg)

![](RackMultipart20210310-4-fcaz0h_html_237499165a11f2b9.gif)

dotAtlas, in essence, is a map-like visualization of 2d points for browsers.

- Customizable colors, sizes, shapes, opacities, elevations and textual labels for all the points.
- Independent control of the elevations, markers, outline and label layers.
- Built-in finding clusters of nearby points for easy multi-point hover and selection.
- WebGL-based implementation for 60 FPS interaction animations, also with large data sets.

There are three ways to get started with dotAtlas:

- [Quick start](https://get.carrotsearch.com/dotatlas/latest/doc/quick-start/): setting up your first simple dotAtlas visualization with a minimal amount of code.
- Guides: in-depth articles covering various aspects of dotAtlas, such as [requirements](https://get.carrotsearch.com/dotatlas/latest/doc/requirements/), [installation](https://get.carrotsearch.com/dotatlas/latest/doc/installation/), [API overview](https://get.carrotsearch.com/dotatlas/latest/doc/api-overview/), [defining layers](https://get.carrotsearch.com/dotatlas/latest/doc/defining-layers/), [listening to events](https://get.carrotsearch.com/dotatlas/latest/doc/listening-to-events/) and more.
- [Tutorial](https://get.carrotsearch.com/dotatlas/latest/doc/tutorial/): step by step instructions on building a more complex dotAtlas visualization, including: layer set-up, handling user interactions and implementing hover and selection highlights.

Finally, the [API](https://get.carrotsearch.com/dotatlas/latest/doc/api-common/)[references](https://get.carrotsearch.com/dotatlas/latest/doc/api-dotatlas/) contain details on all the available options and methods.

### Functions (js)

Key functions that export the authorization and authentication of the user and provide appropriate privileges including project edit, publish &amp; review rights to the user and relevant project(s). Key functions to copy objects simply, user authentication &amp; authorization with regards to the Project resources, check email; URL validity etc.

# Pages

## Admin Pages

## Sub Pages - Components

## Main Pages - Components

# Window Components

## Application Dialogs

### Gallery.vue

Dedicated component uploading images to the project from the local system and prompts warning text when there aren&#39;t any images linked with the project. The component methods include add images, select images, insert images, cancel select images, get image details, load images, delete images with relevant transitions. Load Images (loadImagesPrevNext) leverages Axios GET to immediately send requests to the server including image meta information. ![](RackMultipart20210310-4-fcaz0h_html_f077cc73db64adf8.png)

![](RackMultipart20210310-4-fcaz0h_html_e16d643254e4f464.png)

### VideoProviderChooser.vue

Dedicated component to choose videos to the project from the local system and prompts warning text when there aren&#39;t any images linked with the project. The component methods include validate video links, add video, add images, select video, insert videos, cancel select, get video details, load video, delete video with relevant transitions. Validate video links (validateVideoLink) leverages Axios GET to immediately send requests to the server including links meta information. The function checks the URL validity if the whole URL gets entered or just the shortid of Vimeo or YouTube.

![](RackMultipart20210310-4-fcaz0h_html_1e9f987a764472b.png)

## Mini Windows

### Copy.vue

Specific component for copying resources &amp; cancel using copyObj and runCB methods emitting mini window through custom event bus (VBUS).

![](RackMultipart20210310-4-fcaz0h_html_1d4b755a928dd0d0.png)

### CopyLink.vue

The component that is used in the Project Blog component to copy the link of an added blog entry for easy sharing. The same leverages Props argument to get event &amp; linkid from ProjectBlog.vue to construct the URL(makelink) in format: window.location.origin + &quot;/projects/&quot; + GS.currentprojectid +&quot;/blogentries?b=&quot;+self.args.linkid (e.g. [https://dev.cri-paris.org:43103/projects/VCstJe3S/blogentries?b=603f5697cfd658c33a1b5d51](https://dev.cri-paris.org:43103/projects/VCstJe3S/blogentries?b=603f5697cfd658c33a1b5d51))

![](RackMultipart20210310-4-fcaz0h_html_1fd39c9ea37b6c73.png)

### EditResFile.vue

Specific component to edit each of the file resources using patchRes method through custom event bus (VBUS). The component uses respatch function and passes current obj.\_id along with modified data to the api respatch function.

### ![](RackMultipart20210310-4-fcaz0h_html_ea3bf94f465c7f20.png)

### Edit ResLink.vue

Specific component to edit each of the URL link resources using patchRes method through custom event bus (VBUS). The component uses respatch function and passes current obj.\_id, along with modified data to the api respatch function. The component loops through link categories (resource categories) from the constants file.

![](RackMultipart20210310-4-fcaz0h_html_dc766100d150854e.png)

### EditResProject.vue

Specific component for the mini window to edit each of the Project resources using patchRes method through custom event bus (VBUS). The component uses respatch function and passes current obj.\_id, along with modified data to the api respatch function. The component loops through link categories along with project categories (resource categories from English &amp; French) from the constants file. The same also includes TextInput from shared components to allow the user to annotate the link reason.

![](RackMultipart20210310-4-fcaz0h_html_771c68478cc75ce8.png)

### MiniInfo.vue

Specific component for passing content title &amp; description as argument content&#39;s title &amp; description to Mini window component.

##### ![](RackMultipart20210310-4-fcaz0h_html_e175eddfcddc48c6.png)

### UnsavedData.vue

Specific component for confirming unsaved data of resource using runCB methods emitting mini window close through custom event bus (VBUS).

### YesNo.vue

Specific component for confirming deletion of resource using runCB methods emitting mini window close through custom event bus (VBUS).

![](RackMultipart20210310-4-fcaz0h_html_f570a7cfc1d7555a.png)

#####

## Popup Windows

# Translation Files

# Routing

# Transitions &amp; Animations

# External Libraries

### Vue.js

[Vue.js](https://vuejs.org/) is a javascript web framework.

### TipTap

[TipTap](https://github.com/ueberdosis/tiptap) is a toolkit for building text editors. We are using the vue package for TipTap. TipTap is an extension to [ProseMirror](https://prosemirror.net/) that allows you to create new schemas directly in a vue way.

This editor is used to edit a project&#39;s description or blog post.

### Vue Leaflet

[Vue Leaflet](https://vue2-leaflet.netlify.app/) is a vue package built on Leaflet.

Leaflet is a strong package to build maps and interact with it.

### Vue Color

[Vue Color](https://github.com/xiaokaike/vue-color) is a vue color picker package. It provides a different picker from simple hex code to color choice with opacity.

We are using it to let organization administrators select a background color for categories.

### Axios

[Axios](https://github.com/axios/axios) is an Http client.

We are using it to manage HTTP calls to our API. It is based on promise.

### Drag and resize

[vue-drag-resize](https://github.com/kirillmurashov/vue-drag-resize) is a package made for image resizing and dragging.

We are using it on blog post and description when user upload images or videos

### Bulma

[Bulma](https://bulma.io/) is a CSS framework. We are using the basic version for responsibility and basic component class : Button, Grid etc.

We are also using some components of [Bulma extension](https://bulma.io/extensions/) that bring css/js components like tooltip.

### ChartJs

[vue-chartjs](https://vue-chartjs.org/) is a vue wrapper to Chart.js

We are using it to build chart in Stats page

# State Management

# Server side Rendering

# Backend APIs

### ### api

APIs are registered here. Eve hooks and initialisation.

### ### Authentication

Endpoints about authentication are in `api_auth.py`. 2 authentication was available : CRIID and OPENID. CRIIS is legacy and only OPENID should be used. It should be move in /auth folder

### ### api\_cstm

This file contains all endpoints that are not handled by Eve. Those endpoints are built with Flask and the required package depends on what the service needs to do.

### ### api\_funct

api\_funct\_sec, api\_funct\_mail, api\_funct\_db Tools function. It would be a good idea to create a tools folder and put those file with a better naming

### ### api\_private

Endpoints for server authentication or IP restricted. Used for internal apps communication or client that need to consume data (eg. Organizations)

### ### ref

Reference API. Built to generate accessible projects pages for scrapping (like a custom Server-side-rendering). It will generate meta and project&#39;s images.

### ### settings

Eve configuration file. DB model are represent here with schema and allowed HTTP VERB

### ### migrations

It should contain all DB and file migration. Naming must be link to the version where the migration is needed (eg. v0.3.1)

### ### exceptions

It should contains python specific exceptions we create

### ### TPL

Should contain a flask template. There are used mainly for emails

-------------------------
