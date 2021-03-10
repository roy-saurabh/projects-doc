
<p style="color: red; font-weight: bold">>>>>>  gd2md-html alert:  ERRORs: 0; WARNINGs: 0; ALERTS: 19.</p>

<p style="color: red; font-weight: bold">Links to alert messages:</p><a href="#gdcalert1">alert1</a>
<a href="#gdcalert2">alert2</a>
<a href="#gdcalert3">alert3</a>
<a href="#gdcalert4">alert4</a>
<a href="#gdcalert5">alert5</a>
<a href="#gdcalert6">alert6</a>
<a href="#gdcalert7">alert7</a>
<a href="#gdcalert8">alert8</a>
<a href="#gdcalert9">alert9</a>
<a href="#gdcalert10">alert10</a>
<a href="#gdcalert11">alert11</a>
<a href="#gdcalert12">alert12</a>
<a href="#gdcalert13">alert13</a>
<a href="#gdcalert14">alert14</a>
<a href="#gdcalert15">alert15</a>
<a href="#gdcalert16">alert16</a>
<a href="#gdcalert17">alert17</a>
<a href="#gdcalert18">alert18</a>
<a href="#gdcalert19">alert19</a>

<p style="color: red; font-weight: bold">>>>>> PLEASE check and correct alert issues and delete this message and the inline alerts.<hr></p>


<h2 id="installation">Installation</h2>


Currently there are a lot of dependencies required for a Projects Platform development environment and managing complexity around building Projects Platform Frontend, Backend, CRI People interface, Sockets etc. To mitigate the complexity, we decided to build LXC containers to create a complete environment with all dependencies pre-configured to start contributing to the Projects Platform code in the shortest possible time. 

We replicate the environmental configuration to build a pre-production environment too and make an ISO environment for pre-production and production environment with built-in scripts and access.



1. Create a [SSH key](https://www.ssh.com/ssh/key/) and share the public key with the core user group member with Projects Platform application environment admin access on the main development server. 
2. The admin would add the public key in authorized_keys file and would  create a development environment for the  Projects Platform application that you would now be able to connect to with the provided SSH address _(e.g. : `ssh dev@dev.cri-paris.org -p :<<port#>>`)._
3. Access the directory and explore code folders containing frontend code at  `/WWW/DEV/FRONT` or backend code at `/WWW/DEV/BACK`.
4. Install any IDE of your choice and install either SSH tools to connect from your computer to the remote server or nautilus configuration. (OS dependent)

<h3>Architecture </h3>


The Projects Platform API server is developed in Python using the Flask micro framework. The data & state of the platform are stored in MongoDB. Socket.IO server running under python enables real-time, bidirectional and event-based communication. The client side rendering of DOM of the Project application leverages VueJS and synchronous interactions are managed by the socket.io and prosemirror client libraries.

<h3 id="release-notes">Release Notes</h3>


Latest version: **v0.13.1**

Detailed release notes for each version are available on [GitLab](https://git.cri-paris.org/it-team/project/projects-front/-/tree/release_v0.13.1)

<h4 id="frontend-home">Frontend - Home</h4>


### run FRONT



1. Go to `/WWW/FRONT`
2. Run `npm run dev` your web application will be available on `_https://dev.cri-paris.org:<<port#>>_` Change with the right port of your env !
3. Constants are in `dist/const.js` Some are set up within the env creation. For more details go [here](front/constants.md)

<h4 id="backend-home">Backend - Home</h4>


### run BACK



1. The backend is already running!
2. If something went wrong and you need to re-launch the back process: ‘_sudo touch /etc/uwsgi-emperor/vassals/apiprojectsdev.ini_’. This command needs to be run after any modification of ‘settings.py’.
3. Access logs:  ‘_sudo tail -f /var/log/uwsgi/vassals/apiprojectsdev.log_’.
4. Constants are in ‘_/const.py_’ Some are set up within the env creation. For more details go ‘_back/constants.md_’.

<h4 id="database">Database</h4>


### run MONGO

MongoDB CRUD operations create, read, update, and delete dB documents:



1. To access Mongo CRUD operations, modify dB.
2. Just run `mongo`.
3. Choose the right DB  (default: ‘_apiprojectsdev_’) using ‘use’.
4. Start querying using common commands [here](https://docs.mongodb.com/manual/reference/mongo-shell/)

<h5 id="create-operations">Create Operations</h5>


Create or insert operations add new [documents](https://docs.mongodb.com/manual/core/document/#bson-document-format) to a [collection](https://docs.mongodb.com/manual/core/databases-and-collections/#collections). If the collection does not currently exist, insert operations will create the collection.

MongoDB provides the following methods to insert documents into a collection:



*   [db.collection.insertOne()](https://docs.mongodb.com/manual/reference/method/db.collection.insertOne/#db.collection.insertOne) _New in version 3.2_
*   [db.collection.insertMany()](https://docs.mongodb.com/manual/reference/method/db.collection.insertMany/#db.collection.insertMany) _New in version 3.2_

In MongoDB, insert operations target a single [collection](https://docs.mongodb.com/manual/reference/glossary/#term-collection). All write operations in MongoDB are [atomic](https://docs.mongodb.com/manual/core/write-operations-atomicity/) on the level of a single [document](https://docs.mongodb.com/manual/core/document/).

For examples, see [Insert Documents](https://docs.mongodb.com/manual/tutorial/insert-documents/).

<h5 id="read-operations">Read Operations</h5>


Read operations retrieve [documents](https://docs.mongodb.com/manual/core/document/#bson-document-format) from a [collection](https://docs.mongodb.com/manual/core/databases-and-collections/#collections); i.e. query a collection for documents. MongoDB provides the following methods to read documents from a collection:



*   [db.collection.find()](https://docs.mongodb.com/manual/reference/method/db.collection.find/#db.collection.find)

You can specify [query filters or criteria](https://docs.mongodb.com/manual/tutorial/query-documents/#read-operations-query-argument) that identify the documents to return.

For examples, see:



*   [Query Documents](https://docs.mongodb.com/manual/tutorial/query-documents/)
*   [Query on Embedded/Nested Documents](https://docs.mongodb.com/manual/tutorial/query-embedded-documents/)
*   [Query an Array](https://docs.mongodb.com/manual/tutorial/query-arrays/)
*   [Query an Array of Embedded Documents](https://docs.mongodb.com/manual/tutorial/query-array-of-documents/)

<h5 id="update-operations">Update Operations</h5>


Update operations modify existing [documents](https://docs.mongodb.com/manual/core/document/#bson-document-format) in a [collection](https://docs.mongodb.com/manual/core/databases-and-collections/#collections). MongoDB provides the following methods to update documents of a collection:



*   [db.collection.updateOne()](https://docs.mongodb.com/manual/reference/method/db.collection.updateOne/#db.collection.updateOne) _New in version 3.2_
*   [db.collection.updateMany()](https://docs.mongodb.com/manual/reference/method/db.collection.updateMany/#db.collection.updateMany) _New in version 3.2_
*   [db.collection.replaceOne()](https://docs.mongodb.com/manual/reference/method/db.collection.replaceOne/#db.collection.replaceOne) _New in version 3.2_

In MongoDB, update operations target a single collection. All write operations in MongoDB are [atomic](https://docs.mongodb.com/manual/core/write-operations-atomicity/) on the level of a single document.

You can specify criteria, or filters, that identify the documents to update. These [filters](https://docs.mongodb.com/manual/core/document/#document-query-filter) use the same syntax as read operations.

For examples, see [Update Documents](https://docs.mongodb.com/manual/tutorial/update-documents/).

<h5 id="delete-operations">Delete Operations</h5>


Delete operations remove documents from a collection. MongoDB provides the following methods to delete documents of a collection:



*   [db.collection.deleteOne()](https://docs.mongodb.com/manual/reference/method/db.collection.deleteOne/#db.collection.deleteOne) _New in version 3.2_
*   [db.collection.deleteMany()](https://docs.mongodb.com/manual/reference/method/db.collection.deleteMany/#db.collection.deleteMany) _New in version 3.2_

In MongoDB, delete operations target a single [collection](https://docs.mongodb.com/manual/reference/glossary/#term-collection). All write operations in MongoDB are [atomic](https://docs.mongodb.com/manual/core/write-operations-atomicity/) on the level of a single document.

You can specify criteria, or filters, that identify the documents to remove. These [filters](https://docs.mongodb.com/manual/core/document/#document-query-filter) use the same syntax as read operations.

For examples, see [Delete Documents](https://docs.mongodb.com/manual/tutorial/remove-documents/).

<h5 id="bulk-write">Bulk Write</h5>


MongoDB provides the ability to perform write operations in bulk. For details, see [Bulk Write Operations](https://docs.mongodb.com/manual/core/bulk-write-operations/).

<h4 id="versioning">Versioning</h4>


### GIT

Here you can access the complete documentation for GitLab, the single application for the [entire DevOps lifecycle](https://docs.gitlab.com/ee/README.html#the-entire-devops-lifecycle).

<h5 id="key-relevant-gitlab-documentation">Key relevant GitLab documentation</h5>



<table>
  <tr>
   <td><strong>Essential documentation</strong>
   </td>
   <td><strong>Essential documentation</strong>
   </td>
  </tr>
  <tr>
   <td><a href="https://docs.gitlab.com/ee/user/index.html">User documentation</a>
<p>
Discover features and concepts for GitLab users.
   </td>
   <td><a href="https://docs.gitlab.com/ee/administration/index.html">Administrator documentation</a>
<p>
Everything GitLab self-managed administrators need to know.
   </td>
  </tr>
  <tr>
   <td><a href="https://docs.gitlab.com/ee/README.html#contributing-to-gitlab">Contributing to GitLab</a>
<p>
At GitLab, everyone can contribute!
   </td>
   <td><a href="https://docs.gitlab.com/ee/README.html#new-to-git-and-gitlab">New to Git and GitLab?</a>
<p>
We have the resources to get you started.
   </td>
  </tr>
  <tr>
   <td><a href="https://docs.gitlab.com/ee/README.html#build-an-integration-with-gitlab">Build an integration with GitLab</a>
<p>
Consult our integration documentation.
   </td>
   <td><a href="https://docs.gitlab.com/ee/README.html#coming-to-gitlab-from-another-platform">Coming to GitLab from another platform?</a>
<p>
Consult our guides.
   </td>
  </tr>
  <tr>
   <td><a href="https://about.gitlab.com/install/">Install GitLab</a>
<p>
Installation options for different platforms.
   </td>
   <td><a href="https://docs.gitlab.com/ee/subscriptions/index.html">Customers</a>
<p>
Information for new and existing customers.
   </td>
  </tr>
  <tr>
   <td><a href="https://docs.gitlab.com/ee/update/index.html">Update GitLab</a>
<p>
Update your GitLab self-managed instance to the latest version.
   </td>
   <td><a href="https://docs.gitlab.com/ee/administration/reference_architectures/index.html">Reference Architectures</a>
<p>
GitLab reference architectures.
   </td>
  </tr>
  <tr>
   <td><a href="https://about.gitlab.com/releases/">GitLab releases</a>
<p>
What’s new in GitLab.
   </td>
   <td> 
   </td>
  </tr>
</table>


<h5 id="popular-topics">Popular topics</h5>


Have a look at some of our most popular topics:


<table>
  <tr>
   <td><strong>Popular topic</strong>
   </td>
   <td><strong>Description</strong>
   </td>
  </tr>
  <tr>
   <td><a href="https://docs.gitlab.com/ee/user/profile/account/two_factor_authentication.html">Two-factor authentication</a>
   </td>
   <td>Improve the security of your GitLab account.
   </td>
  </tr>
  <tr>
   <td><a href="https://docs.gitlab.com/ee/user/group/index.html">GitLab groups</a>
   </td>
   <td>Manage projects together.
   </td>
  </tr>
  <tr>
   <td><a href="https://docs.gitlab.com/ee/ci/yaml/README.html">GitLab CI/CD pipeline configuration reference</a>
   </td>
   <td>Available configuration options for .gitlab-ci.yml files.
   </td>
  </tr>
  <tr>
   <td><a href="https://docs.gitlab.com/ee/user/admin_area/license.html">Activate GitLab EE with a license</a>
   </td>
   <td>Activate GitLab Enterprise Edition functionality with a license.
   </td>
  </tr>
  <tr>
   <td><a href="https://docs.gitlab.com/ee/raketasks/backup_restore.html">Back up and restore GitLab</a>
   </td>
   <td>Rake tasks for backing up and restoring GitLab self-managed instances.
   </td>
  </tr>
  <tr>
   <td><a href="https://docs.gitlab.com/ee/policy/maintenance.html">GitLab release and maintenance policy</a>
   </td>
   <td>Policies for version naming and cadence, and also upgrade recommendations.
   </td>
  </tr>
  <tr>
   <td><a href="https://docs.gitlab.com/ee/integration/elasticsearch.html">Elasticsearch integration</a>
   </td>
   <td>Integrate Elasticsearch with GitLab to enable advanced searching.
   </td>
  </tr>
  <tr>
   <td><a href="https://docs.gitlab.com/omnibus/settings/database.html">Omnibus GitLab database settings</a>
   </td>
   <td>Database settings for Omnibus GitLab self-managed instances.
   </td>
  </tr>
  <tr>
   <td><a href="https://docs.gitlab.com/omnibus/settings/nginx.html">Omnibus GitLab NGINX settings</a>
   </td>
   <td>NGINX settings for Omnibus GitLab self-managed instances.
   </td>
  </tr>
  <tr>
   <td><a href="https://docs.gitlab.com/omnibus/settings/ssl.html">Omnibus GitLab SSL configuration</a>
   </td>
   <td>SSL settings for Omnibus GitLab self-managed instances.
   </td>
  </tr>
  <tr>
   <td><a href="https://docs.gitlab.com/ee/user/gitlab_com/index.html">GitLab.com settings</a>
   </td>
   <td>Settings used for GitLab.com.
   </td>
  </tr>
</table>


<h5 id="the-entire-devops-lifecycle">The entire DevOps lifecycle</h5>


GitLab is the application for software development, security, and operations that enables [Concurrent DevOps](https://about.gitlab.com/topics/concurrent-devops/). GitLab makes the software lifecycle faster and radically improves the speed of business. Git is directly configured so you can add your own gitlab CRI alias and start creating your own feature branch.

<h2 id="introduction">Introduction</h2>


Projects platform to reference a community's projects and is home to a community of passionate, inspiring projects that are launched there every day.

Nevertheless, it is difficult to know what is going on there every day, and we all "miss" many daily achievements. Because of a lack of visibility, some projects lose the opportunity for better support, and precious resources are spent on redundant ideas.

<h4 id="helping-the-community">Helping the community</h4>


We believe that it will also make it easier to train teams on certain subjects by allowing them to better identify the skills and achievements already available or in gestation.

It is also a way to get to know the people in the community or who revolve around the organization and its projects, in line with the objectives of sustainable development defined by the United Nations.

<h4 id="communicate-better">Communicate better</h4>


This platform will enhance the organization's impact by simply presenting the extent of its creative force and potential.

This will benefit everyone, with each project benefiting from centralized and broader communication.

Indeed Projects Platform is, as well as CRI people, a data source for all CRI's digital means of communication, avoiding - badly - duplicated information.

<h4 id="what-fields-are-included-in-a-project">What fields are included in a project?</h4>


When you create a new project, you create a title, an image, contributors and you can annotate it by UNESCO's sustainable development objectives to which it is addressed and by keywords. These keywords are chosen from all available Wikipedia article titles. They make it easy to find projects with similarities. In the following, they will also be visualized and shared on the WeLearn cartography.

<h3 id="what-is-a-projects-platform">What is a Projects Platform?</h3>


In order to better share ideas worth sharing with everyone, we have created the Projects platform for presentation and referencing of all projects that are  intended to be collaborative and easy to access, it will allow everyone to have a directory of the many projects carried out and to present their own achievements.

We also believe that other organizations have the same need for better project sharing. We propose that they benefit from this tool.

<h4 id="getting-started">Getting Started</h4>


<h5 id="our-current-projects-platform-folder-structure">Our current Projects platform folder structure</h5>


<h5 id="key-folders">**Key Folders**</h5>


<h6 id="application-dialogs-appdialogs">Application Dialogs (appdialogs)</h6>


Pop-in component for Description and Blog. Vue component inside should be moved in shrcomponents or wins

<h6 id="assets-assets">Assets (assets)</h6>


Fonts and global images. Warning : Images are now in a file system based so no new images should be added here and the /img subfolder might be deleted.

<h6 id="global-functions-functs">Global Functions (functs)</h6>


Global function that can be reused. It should contain services. Some functions might be added in a mixin.

<h6>Mixins (mixins) </h6>


Component function that can be added in more than one component. Refers to vue documentation to understand the meaning of a mixin.

<h6 id="mini-pop-in-windows-miniwins">Mini Pop-in Windows(miniwins)</h6>


Small pop-in component. It would be better to have few functional pop-in component and inject only text in it.

<h6 id="pages-pages">Pages (pages)</h6>


It should only contain user pages and those pages components should be built with other component.

<h6 id="popups-popups">Popups (popups)</h6>


Popup components

<h6 id="scss-scss">SCSS (scss)</h6>


SCSS global files

<h6 id="shared-components-shrcomponents">Shared Components (shrcomponents)</h6>


All reusable components. All components expect pages and one used component should be here. Even wins and miniwins.

<h6 id="windows-wins">Windows (wins)</h6>


Large pop-in components

<h5 id="custom-vue-event-bus-vbus">**Custom Vue Event Bus (VBUS)**</h5>


To understand VBUS is critical to understand Projects Platform component event communication. We currently don’t use Vuex that could be a better way to manage state and data flow across components. We are utilizing VBUS currently to connect unrelated sections of our VueJs Application/Codebase talk to each other with current project code  event bus/publisher-subscriber pattern. The same has provided flexibility to have communication between unrelated or sibling relationships but can very easily create ambiguous and unmanageable state management within an application as complex as the Projects Platform. So the next stage of optimization of Projects would include re-architecting the application and include Vuex to alter a global state that all components check for via getters instead of VBUS.

So then in a completely unrelated component you would need to hook into that event and react to it, I find myself registering the event hooks in the components mounted() lifecycle hook to be able to listen to events. Similar to child to parent communication but the difference is the component reacting to the event registers its listener in a different place (in this case in the mounted hook). Now you have the ability for one component to speak to another component in a different part of your application. It is a handy thing to know but of course beware of overusing this. It could get mucky or used where a different approach might better suit. So these event systems come part and parcel of Vue and can be utilised to achieve component communication in a variety of ways.

The Publisher-Subscriber pattern we will use to allow components to subscribe to an event. Then other components can publish an event and all subscribers can then react to that. Two main methods to allow subscription and the ability to publish to those subscribers. Again this then means we get access in every component to the PubSub instance via this.$pubSub. So then we must subscribe to some components, a good example would be a bunch of show/hide panel components, they all can open independently. You wish to have a button elsewhere in the application that you would want to have the ability to close all those other panel components with one click. So here we see that we will use mounted() to subscribe to an event called closePanels. When it is invoked then we will run our localMethod to close the panel. So this time our click event will run this. $pubSub.publish(‘closePanels’), which will inform all subscribers to run and thus close them all. We have run through different ways to utilise communication throughout your VueJs Application. We have used event systems and we have used some patterns to help the way these components communicate. Again it is trying to find the right time to use each and when.

<h2 id="application-&-component-instances">Application & Component Instances</h2>


<h3 id="creating-an-application-instance">Creating an Application Instance</h3>


Every Vue application starts by creating a new application instance with the createApp function:

const app = Vue.createApp({

  /* options */

})

The application instance is used to register 'globals' that can then be used by components within that application. We'll discuss that in detail later in the guide but as a quick example:

const app = Vue.createApp({})

app.component('SearchInput', SearchInputComponent)

app.directive('focus', FocusDirective)

app.use(LocalePlugin)

Most of the methods exposed by the application instance return that same instance, allowing for chaining:

Vue.createApp({})

  .component('SearchInput', SearchInputComponent)

  .directive('focus', FocusDirective)

  .use(LocalePlugin)

You can browse the full application API in the [API reference](https://v3.vuejs.org/api/application-api.html).

<h3 id="#the-root-component">
[#](https://v3.vuejs.org/guide/instance.html#the-root-component)The Root Component</h3>


The options passed to createApp are used to configure the root component. That component is used as the starting point for rendering when we mount the application.

An application needs to be mounted into a DOM element. For example, if we want to mount a Vue application into <div id="app"></div>, we should pass #app:

const RootComponent = {

  /* options */

}

const app = Vue.createApp(RootComponent)

const vm = app.mount('#app')

Unlike most of the application methods, mount does not return the application. Instead it returns the root component instance.

Although not strictly associated with the [MVVM pattern](https://en.wikipedia.org/wiki/Model_View_ViewModel), Vue's design was partly inspired by it. As a convention, we often use the variable vm (short for ViewModel) to refer to a component instance.

While all the examples on this page only need a single component, most real applications are organized into a tree of nested, reusable components. For example, a Todo application's component tree might look like this:

Root Component

└─ TodoList

   ├─ TodoItem

   │  ├─ DeleteTodoButton

   │  └─ EditTodoButton

   └─ TodoListFooter

      ├─ ClearTodosButton

      └─ TodoListStatistics

Each component will have its own component instance, vm. For some components, such as TodoItem, there will likely be multiple instances rendered at any one time. All of the component instances in this application will share the same application instance.

We'll talk about [the component system](https://v3.vuejs.org/guide/component-basics.html) in detail later. For now, just be aware that the root component isn't really any different from any other component. The configuration options are the same, as is the behavior of the corresponding component instance.

<h3 id="#component-instance-properties">
[#](https://v3.vuejs.org/guide/instance.html#component-instance-properties)Component Instance Properties</h3>


Earlier in the guide we met data properties. Properties defined in data are exposed via the component instance:

const app = Vue.createApp({

  data() {

    return { count: 4 }

  }

})

const vm = app.mount('#app')

console.log(vm.count) // => 4

There are various other component options that add user-defined properties to the component instance, such as methods, props, computed, inject and setup. We'll discuss each of these in depth later in the guide. All of the properties of the component instance, no matter how they are defined, will be accessible in the component's template.

Vue also exposes some built-in properties via the component instance, such as $attrs and $emit. These properties all have a $ prefix to avoid conflicting with user-defined property names.

<h3 id="#lifecycle-hooks">
[#](https://v3.vuejs.org/guide/instance.html#lifecycle-hooks)Lifecycle Hooks</h3>


Each component instance goes through a series of initialization steps when it's created - for example, it needs to set up data observation, compile the template, mount the instance to the DOM, and update the DOM when data changes. Along the way, it also runs functions called lifecycle hooks, giving users the opportunity to add their own code at specific stages.

For example, the [created](https://v3.vuejs.org/api/options-lifecycle-hooks.html#created) hook can be used to run code after an instance is created:

Vue.createApp({

  data() {

    return { count: 1 }

  },

  created() {

    // `this` points to the vm instance

    console.log('count is: ' + this.count) // => "count is: 1"

  }

})

There are also other hooks which will be called at different stages of the instance's lifecycle, such as [mounted](https://v3.vuejs.org/api/options-lifecycle-hooks.html#mounted), [updated](https://v3.vuejs.org/api/options-lifecycle-hooks.html#updated), and [unmounted](https://v3.vuejs.org/api/options-lifecycle-hooks.html#unmounted). All lifecycle hooks are called with this context pointing to the current active instance invoking it

Don't use [arrow functions ](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Functions/Arrow_functions)on an options property or callback, such as created: () => console.log(this.a) or vm.$watch('a', newValue => this.myMethod()). Since an arrow function doesn't have a this, this will be treated as any other variable and lexically looked up through parent scopes until found, often resulting in errors such as Uncaught TypeError: Cannot read property of undefined or Uncaught TypeError: this.myMethod is not a function.

<h3 id="#lifecycle-diagram">
[#](https://v3.vuejs.org/guide/instance.html#lifecycle-diagram)Lifecycle Diagram</h3>


Below is a diagram for the instance lifecycle. You don't need to fully understand everything going on right now, but as you learn and build more, it will be a useful reference.

<h2 id="template-syntax">Template Syntax</h2>


Vue.js uses an HTML-based template syntax that allows you to declaratively bind the rendered DOM to the underlying component instance's data. All Vue.js templates are valid HTML that can be parsed by spec-compliant browsers and HTML parsers.

Under the hood, Vue compiles the templates into Virtual DOM render functions. Combined with the reactivity system, Vue is able to intelligently figure out the minimal number of components to re-render and apply the minimal amount of DOM manipulations when the app state changes.

If you are familiar with Virtual DOM concepts and prefer the raw power of JavaScript, you can also [directly write render functions](https://v3.vuejs.org/guide/render-function.html) instead of templates, with optional JSX support.

<h3 id="#interpolations">
[#](https://v3.vuejs.org/guide/template-syntax.html#interpolations)Interpolations</h3>


<h4 id="#text">
[#](https://v3.vuejs.org/guide/template-syntax.html#text)Text</h4>


The most basic form of data binding is text interpolation using the "Mustache" syntax (double curly braces):

<span>Message: {{ msg }}</span>

The mustache tag will be replaced with the value of the msg property from the corresponding component instance. It will also be updated whenever the msg property changes.

You can also perform one-time interpolations that do not update on data change by using the [v-once directive](https://v3.vuejs.org/api/directives.html#v-once), but keep in mind this will also affect any other bindings on the same node:

<span v-once>This will never change: {{ msg }}</span>

<h4 id="#raw-html">
[#](https://v3.vuejs.org/guide/template-syntax.html#raw-html)Raw HTML</h4>


The double mustaches interpret the data as plain text, not HTML. In order to output real HTML, you will need to use the [v-html directive](https://v3.vuejs.org/api/directives.html#v-html):

<p>Using mustaches: {{ rawHtml }}</p>

<p>Using v-html directive: <span v-html="rawHtml"></span></p>

The contents of the span will be replaced with the value of the rawHtml property, interpreted as plain HTML - data bindings are ignored. Note that you cannot use v-html to compose template partials, because Vue is not a string-based templating engine. Instead, components are preferred as the fundamental unit for UI reuse and composition.

TIP

Dynamically rendering arbitrary HTML on your website can be very dangerous because it can easily lead to XSS vulnerabilities

. Only use HTML interpolation on trusted content and never on user-provided content

<h4 id="#attributes">
[#](https://v3.vuejs.org/guide/template-syntax.html#attributes)Attributes</h4>


Mustaches cannot be used inside HTML attributes. Instead, use a [v-bind directive](https://v3.vuejs.org/api/directives.html#v-bind):

<div v-bind:id="dynamicId"></div>

If the bound value is null or undefined then the attribute will not be included on the rendered element.

In the case of boolean attributes, where their mere existence implies true, v-bind works a little differently. For example:

<button v-bind:disabled="isButtonDisabled">Button</button>

The disabled attribute will be included if isButtonDisabled has a truthy value. It will also be included if the value is an empty string, maintaining consistency with <button disabled="">. For other falsy values the attribute will be omitted.

<h4 id="#using-javascript-expressions">
[#](https://v3.vuejs.org/guide/template-syntax.html#using-javascript-expressions)Using JavaScript Expressions</h4>


So far we've only been binding to simple property keys in our templates. But Vue.js actually supports the full power of JavaScript expressions inside all data bindings:

{{ number + 1 }}

{{ ok ? 'YES' : 'NO' }}

{{ message.split('').reverse().join('') }}

<div v-bind:id="'list-' + id"></div>

These expressions will be evaluated as JavaScript in the data scope of the current active instance. One restriction is that each binding can only contain one single expression, so the following will NOT work:

<!-- this is a statement, not an expression: -->

{{ var a = 1 }}

<!-- flow control won't work either, use ternary expressions -->

{{ if (ok) { return message } }}

<h3 id="#directives">
[#](https://v3.vuejs.org/guide/template-syntax.html#directives)Directives</h3>


Directives are special attributes with the v- prefix. Directive attribute values are expected to be a single JavaScript expression (with the exception of v-for and v-on, which will be discussed later). A directive's job is to reactively apply side effects to the DOM when the value of its expression changes. Let's review the example we saw in the introduction:

<p v-if="seen">Now you see me</p>

Here, the v-if directive would remove/insert the <p> element based on the truthiness of the value of the expression seen.

<h4 id="#arguments">
[#](https://v3.vuejs.org/guide/template-syntax.html#arguments)Arguments</h4>


Some directives can take an "argument", denoted by a colon after the directive name. For example, the v-bind directive is used to reactively update an HTML attribute:

<a v-bind:href="url"> ... </a>

Here href is the argument, which tells the v-bind directive to bind the element's href attribute to the value of the expression url.

Another example is the v-on directive, which listens to DOM events:

<a v-on:click="doSomething"> ... </a>

Here the argument is the event name to listen to. We will talk about event handling in more detail too.

<h4 id="#dynamic-arguments">
[#](https://v3.vuejs.org/guide/template-syntax.html#dynamic-arguments)Dynamic Arguments</h4>


It is also possible to use a JavaScript expression in a directive argument by wrapping it with square brackets:

<!--

Note that there are some constraints to the argument expression, as explained

in the "Dynamic Argument Expression Constraints" section below.

-->

<a v-bind:[attributeName]="url"> ... </a>

Here attributeName will be dynamically evaluated as a JavaScript expression, and its evaluated value will be used as the final value for the argument. For example, if your component instance has a data property, attributeName, whose value is "href", then this binding will be equivalent to v-bind:href.

Similarly, you can use dynamic arguments to bind a handler to a dynamic event name:

<a v-on:[eventName]="doSomething"> ... </a>

In this example, when eventName's value is "focus", v-on:[eventName] will be equivalent to v-on:focus.

<h4 id="#modifiers">
[#](https://v3.vuejs.org/guide/template-syntax.html#modifiers)Modifiers</h4>


Modifiers are special postfixes denoted by a dot, which indicate that a directive should be bound in some special way. For example, the .prevent modifier tells the v-on directive to call event.preventDefault() on the triggered event:

<form v-on:submit.prevent="onSubmit">...</form>

You'll see other examples of modifiers later, [for v-on](https://v3.vuejs.org/guide/events.html#event-modifiers) and [for v-model](https://v3.vuejs.org/guide/forms.html#modifiers), when we explore those features.

<h3 id="#shorthands">
[#](https://v3.vuejs.org/guide/template-syntax.html#shorthands)Shorthands</h3>


The v- prefix serves as a visual cue for identifying Vue-specific attributes in your templates. This is useful when you are using Vue.js to apply dynamic behavior to some existing markup, but can feel verbose for some frequently used directives. At the same time, the need for the v- prefix becomes less important when you are building a [SPA](https://en.wikipedia.org/wiki/Single-page_application), where Vue manages every template. Therefore, Vue provides special shorthands for two of the most often used directives, v-bind and v-on:

[#](https://v3.vuejs.org/guide/template-syntax.html#v-bind-shorthand)v-bind 

<!-- full syntax -->

<a v-bind:href="url"> ... </a>

<!-- shorthand -->

<a :href="url"> ... </a>

<!-- shorthand with dynamic argument -->

<a :[key]="url"> ... </a>

[#](https://v3.vuejs.org/guide/template-syntax.html#v-on-shorthand)v-on Shorthand

<!-- full syntax -->

<a v-on:click="doSomething"> ... </a>

<!-- shorthand -->

<a @click="doSomething"> ... </a>

<!-- shorthand with dynamic argument -->

<a @[event]="doSomething"> ... </a>

They may look a bit different from normal HTML, but : and @ are valid characters for attribute names and all Vue-supported browsers can parse it correctly. In addition, they do not appear in the final rendered markup. The shorthand syntax is totally optional, but you will likely appreciate it when you learn more about its usage later.

<h4 id="#caveats">
[#](https://v3.vuejs.org/guide/template-syntax.html#caveats)Caveats</h4>


<h5 id="#dynamic-argument-value-constraints">
[#](https://v3.vuejs.org/guide/template-syntax.html#dynamic-argument-value-constraints)Dynamic Argument Value Constraints</h5>


Dynamic arguments are expected to evaluate to a string, with the exception of null. The special value null can be used to explicitly remove the binding. Any other non-string value will trigger a warning.

<h5 id="#dynamic-argument-expression-constraints">
[#](https://v3.vuejs.org/guide/template-syntax.html#dynamic-argument-expression-constraints)Dynamic Argument Expression Constraints</h5>


Dynamic argument expressions have some syntax constraints because certain characters, such as spaces and quotes, are invalid inside HTML attribute names. For example, the following is invalid:

<!-- This will trigger a compiler warning. -->

<a v-bind:['foo' + bar]="value"> ... </a>

We recommend replacing any complex expressions with a [computed property](https://v3.vuejs.org/guide/computed.html), one of the most fundamental pieces of Vue, which we'll cover shortly.

When using in-DOM templates (templates directly written in an HTML file), you should also avoid naming keys with uppercase characters, as browsers will coerce attribute names into lowercase:

<!--

This will be converted to v-bind:[someattr] in in-DOM templates.

Unless you have a "someattr" property in your instance, your code won't work.

-->

<a v-bind:[someAttr]="value"> ... </a>

Template expressions are sandboxed and only have access to a [whitelist of globals ](https://github.com/vuejs/vue-next/blob/master/packages/shared/src/globalsWhitelist.ts#L3)

such as Math and Date. You should not attempt to access user defined globals in template expressions.

<h2 id="data-properties-and-methods">Data Properties and Methods</h2>


<h3 id="#data-properties">
[#](https://v3.vuejs.org/guide/data-methods.html#data-properties)Data Properties</h3>


The data option for a component is a function. Vue calls this function as part of creating a new component instance. It should return an object, which Vue will then wrap in its reactivity system and store on the component instance as $data. For convenience, any top-level properties of that object are also exposed directly via the component instance:

const app = Vue.createApp({

  data() {

    return { count: 4 }

  }

})

const vm = app.mount('#app')

console.log(vm.$data.count) // => 4

console.log(vm.count)       // => 4

// Assigning a value to vm.count will also update $data.count

vm.count = 5

console.log(vm.$data.count) // => 5

// ... and vice-versa

vm.$data.count = 6

console.log(vm.count) // => 6

These instance properties are only added when the instance is first created, so you need to ensure they are all present in the object returned by the data function. Where necessary, use null, undefined or some other placeholder value for properties where the desired value isn't yet available.

It is possible to add a new property directly to the component instance without including it in data. However, because this property isn't backed by the reactive $data object, it won't automatically be tracked by [Vue's reactivity system](https://v3.vuejs.org/guide/reactivity.html).

Vue uses a $ prefix when exposing its own built-in APIs via the component instance. It also reserves the prefix _ for internal properties. You should avoid using names for top-level data properties that start with either of these characters.

<h3 id="#methods">
[#](https://v3.vuejs.org/guide/data-methods.html#methods)Methods</h3>


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

const vm = app.mount('#app')

console.log(vm.count) // => 4

vm.increment()

console.log(vm.count) // => 5

Vue automatically binds the this value for methods so that it always refers to the component instance. This ensures that a method retains the correct this value if it's used as an event listener or callback. You should avoid using arrow functions when defining methods, as that prevents Vue from binding the appropriate this value.

Just like all other properties of the component instance, the methods are accessible from within the component's template. Inside a template they are most commonly used as event listeners:

<button @click="increment">Up vote</button>

In the example above, the method increment will be called when the <button> is clicked.

It is also possible to call a method directly from a template. As we'll see shortly, it's usually better to use a [computed property](https://v3.vuejs.org/guide/computed.html) instead. However, using a method can be useful in scenarios where computed properties aren't a viable option. You can call a method anywhere that a template supports JavaScript expressions:

<span :title="toTitleDate(date)">

  {{ formatDate(date) }}

</span>

If the methods toTitleDate or formatDate access any reactive data then it will be tracked as a rendering dependency, just as if it had been used in the template directly.

Methods called from a template should not have any side effects, such as changing data or triggering asynchronous processes. If you find yourself tempted to do that you should probably use a [lifecycle hook](https://v3.vuejs.org/guide/instance.html#lifecycle-hooks) instead.

[#](https://v3.vuejs.org/guide/data-methods.html#debouncing-and-throttling)Debouncing and Throttling

Vue doesn't include built-in support for debouncing or throttling but it can be implemented using libraries such as [Lodash](https://lodash.com/).

In cases where a component is only used once, the debouncing can be applied directly within methods:

<script src="https://unpkg.com/lodash@4.17.20/lodash.min.js"></script>

<script>

  Vue.createApp({

    methods: {

      // Debouncing with Lodash

      click: _.debounce(function() {

        // ... respond to click ...

      }, 500)

    }

  }).mount('#app')

</script>

However, this approach is potentially problematic for components that are reused because they'll all share the same debounced function. To keep the component instances independent from each other, we can add the debounced function in the created lifecycle hook:

app.component('save-button', {

  created() {

    // Debouncing with Lodash

    this.debouncedClick = _.debounce(this.click, 500)

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

    <button @click="debouncedClick">

     Save

    </button>

  `

})

<h2 id="computed-properties-and-watchers">Computed Properties and Watchers</h2>


<h3 id="#computed-properties">
[#](https://v3.vuejs.org/guide/computed.html#computed-properties)Computed Properties</h3>


In-template expressions are very convenient, but they are meant for simple operations. Putting too much logic in your templates can make them bloated and hard to maintain. For example, if we have an object with a nested array:

Vue.createApp({

  data() {

    return {

      author: {

        name: 'John Doe',

        books: [

          'Vue 2 - Advanced Guide',

          'Vue 3 - Basic Guide',

          'Vue 4 - The Mystery'

        ]

      }

    }

  }

})

And we want to display different messages depending on if author already has some books or not

<div id="computed-basics">

  <p>Has published books:</p>

  <span>{{ author.books.length > 0 ? 'Yes' : 'No' }}</span>

</div>

At this point, the template is no longer simple and declarative. You have to look at it for a second before realizing that it performs a calculation depending on author.books. The problem is made worse when you want to include this calculation in your template more than once.

That's why for complex logic that includes reactive data, you should use a computed property.

<h4 id="#basic-example">
[#](https://v3.vuejs.org/guide/computed.html#basic-example)Basic Example</h4>


<div id="computed-basics">

  <p>Has published books:</p>

  <span>{{ publishedBooksMessage }}</span>

</div>

Vue.createApp({

  data() {

    return {

      author: {

        name: 'John Doe',

        books: [

          'Vue 2 - Advanced Guide',

          'Vue 3 - Basic Guide',

          'Vue 4 - The Mystery'

        ]

      }

    }

  },

  computed: {

    // a computed getter

    publishedBooksMessage() {

      // `this` points to the vm instance

      return this.author.books.length > 0 ? 'Yes' : 'No'

    }

  }

}).mount('#computed-basics')

Result:

Here we have declared a computed property publishedBooksMessage.

Try to change the value of books array in the application data and you will see how publishedBooksMessage is changing accordingly.

You can data-bind to computed properties in templates just like a normal property. Vue is aware that vm.publishedBooksMessage depends on vm.author.books, so it will update any bindings that depend on vm.publishedBooksMessage when vm.author.books changes. And the best part is that we've created this dependency relationship declaratively: the computed getter function has no side effects, which makes it easier to test and understand.

<h4 id="#computed-caching-vs-methods">
[#](https://v3.vuejs.org/guide/computed.html#computed-caching-vs-methods)Computed Caching vs Methods</h4>


You may have noticed we can achieve the same result by invoking a method in the expression:

<p>{{ calculateBooksMessage() }}</p>

// in component

methods: {

  calculateBooksMessage() {

    return this.author.books.length > 0 ? 'Yes' : 'No'

  }

}

Instead of a computed property, we can define the same function as a method. For the end result, the two approaches are indeed exactly the same. However, the difference is that computed properties are cached based on their reactive dependencies. A computed property will only re-evaluate when some of its reactive dependencies have changed. This means as long as author.books has not changed, multiple access to the publishedBooksMessage computed property will immediately return the previously computed result without having to run the function again.

This also means the following computed property will never update, because Date.now() is not a reactive dependency:

computed: {

  now() {

    return Date.now()

  }

}

In comparison, a method invocation will always run the function whenever a re-render happens.

Why do we need caching? Imagine we have an expensive computed property list, which requires looping through a huge array and doing a lot of computations. Then we may have other computed properties that in turn depend on list. Without caching, we would be executing list’s getter many more times than necessary! In cases where you do not want caching, use a method instead.

<h4 id="#computed-setter">
[#](https://v3.vuejs.org/guide/computed.html#computed-setter)Computed Setter</h4>


Computed properties are by default getter-only, but you can also provide a setter when you need it:

// ...

computed: {

  fullName: {

    // getter

    get() {

      return this.firstName + ' ' + this.lastName

    },

    // setter

    set(newValue) {

      const names = newValue.split(' ')

      this.firstName = names[0]

      this.lastName = names[names.length - 1]

    }

  }

}

// ...

Now when you run vm.fullName = 'John Doe', the setter will be invoked and vm.firstName and vm.lastName will be updated accordingly.

<h3 id="#watchers">
[#](https://v3.vuejs.org/guide/computed.html#watchers)Watchers</h3>


While computed properties are more appropriate in most cases, there are times when a custom watcher is necessary. That's why Vue provides a more generic way to react to data changes through the watch option. This is most useful when you want to perform asynchronous or expensive operations in response to changing data.

For example:

<div id="watch-example">

  <p>

    Ask a yes/no question:

    <input v-model="question" />

  </p>

  <p>{{ answer }}</p>

</div>

<!-- Since there is already a rich ecosystem of ajax libraries    -->

<!-- and collections of general-purpose utility methods, Vue core -->

<!-- is able to remain small by not reinventing them. This also   -->

<!-- gives you the freedom to use what you're familiar with.      -->

<script src="https://cdn.jsdelivr.net/npm/axios@0.12.0/dist/axios.min.js"></script>

<script>

  const watchExampleVM = Vue.createApp({

    data() {

      return {

        question: '',

        answer: 'Questions usually contain a question mark. ;-)'

      }

    },

    watch: {

      // whenever question changes, this function will run

      question(newQuestion, oldQuestion) {

        if (newQuestion.indexOf('?') > -1) {

          this.getAnswer()

        }

      }

    },

    methods: {

      getAnswer() {

        this.answer = 'Thinking...'

        axios

          .get('https://yesno.wtf/api')

          .then(response => {

            this.answer = response.data.answer

          })

          .catch(error => {

            this.answer = 'Error! Could not reach the API. ' + error

          })

      }

    }

  }).mount('#watch-example')

</script>

Result:

In this case, using the watch option allows us to perform an asynchronous operation (accessing an API) and sets a condition for performing this operation. None of that would be possible with a computed property.

In addition to the watch option, you can also use the imperative [vm.$watch API](https://v3.vuejs.org/api/instance-methods.html#watch).

<h4 id="#computed-vs-watched-property">
[#](https://v3.vuejs.org/guide/computed.html#computed-vs-watched-property)Computed vs Watched Property</h4>


Vue does provide a more generic way to observe and react to data changes on a current active instance: watch properties. When you have some data that needs to change based on some other data, it is tempting to overuse watch - especially if you are coming from an AngularJS background. However, it is often a better idea to use a computed property rather than an imperative watch callback. Consider this example:

<div id="demo">{{ fullName }}</div>

const vm = Vue.createApp({

  data() {

    return {

      firstName: 'Foo',

      lastName: 'Bar',

      fullName: 'Foo Bar'

    }

  },

  watch: {

    firstName(val) {

      this.fullName = val + ' ' + this.lastName

    },

    lastName(val) {

      this.fullName = this.firstName + ' ' + val

    }

  }

}).mount('#demo')

The above code is imperative and repetitive. Compare it with a computed property version:

const vm = Vue.createApp({

  data() {

    return {

      firstName: 'Foo',

      lastName: 'Bar'

    }

  },

  computed: {

    fullName() {

      return this.firstName + ' ' + this.lastName

    }

  }

}).mount('#demo')

Much better, isn't it?

<h2 id="class-and-style-bindings">Class and Style Bindings</h2>


A common need for data binding is manipulating an element's class list and its inline styles. Since they are both attributes, we can use v-bind to handle them: we only need to calculate a final string with our expressions. However, meddling with string concatenation is annoying and error-prone. For this reason, Vue provides special enhancements when v-bind is used with class and style. In addition to strings, the expressions can also evaluate to objects or arrays.

<h3 id="#binding-html-classes">
[#](https://v3.vuejs.org/guide/class-and-style.html#binding-html-classes)Binding HTML Classes</h3>


<h4 id="#object-syntax">
[#](https://v3.vuejs.org/guide/class-and-style.html#object-syntax)Object Syntax</h4>


We can pass an object to :class (short for v-bind:class) to dynamically toggle classes:

<div :class="{ active: isActive }"></div>

The above syntax means the presence of the active class will be determined by the [truthiness ](https://developer.mozilla.org/en-US/docs/Glossary/Truthy)


[(opens new window)](https://developer.mozilla.org/en-US/docs/Glossary/Truthy)

of the data property isActive.

You can have multiple classes toggled by having more fields in the object. In addition, the :class directive can also co-exist with the plain class attribute. So given the following template:

<div

  class="static"


<p id="gdcalert1" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert2">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


  :class="{ active: isActive, 'text-danger': hasError }"

></div>

And the following data:

data() {

  return {

    isActive: true,

    hasError: false

  }

}

It will render:

<div class="static active"></div>

When isActive or hasError changes, the class list will be updated accordingly. For example, if hasError becomes true, the class list will become "static active text-danger".

The bound object doesn't have to be inline:

<div :class="classObject"></div>

data() {

  return {

    classObject: {

      active: true,

      'text-danger': false

    }

  }

}

This will render the same result. We can also bind to a [computed property](https://v3.vuejs.org/guide/computed.html) that returns an object. This is a common and powerful pattern:

<div :class="classObject"></div>

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

      'text-danger': this.error && this.error.type === 'fatal'

    }

  }

}

<h4 id="#array-syntax">
[#](https://v3.vuejs.org/guide/class-and-style.html#array-syntax)Array Syntax</h4>


We can pass an array to :class to apply a list of classes:

<div :class="[activeClass, errorClass]"></div>

data() {

  return {

    activeClass: 'active',

    errorClass: 'text-danger'

  }

}

Which will render:

<div class="active text-danger"></div>

If you would like to also toggle a class in the list conditionally, you can do it with a ternary expression:

<div :class="[isActive ? activeClass : '', errorClass]"></div>

This will always apply errorClass, but activeClass will only be applied when isActive is truthy.

However, this can be a bit verbose if you have multiple conditional classes. That's why it's also possible to use the object syntax inside array syntax:

<div :class="[{ active: isActive }, errorClass]"></div>

<h4 id="#with-components">
[#](https://v3.vuejs.org/guide/class-and-style.html#with-components)With Components</h4>


When you use the class attribute on a custom component with a single root element, those classes will be added to this element. Existing classes on this element will not be overwritten.

For example, if you declare this component:

const app = Vue.createApp({})

app.component('my-component', {

  template: `<p class="foo bar">Hi!</p>`

})

Then add some classes when using it:

<div id="app">

  <my-component class="baz boo"></my-component>

</div>

The rendered HTML will be:

<p class="foo bar baz boo">Hi</p>

The same is true for class bindings:

<my-component :class="{ active: isActive }"></my-component>

When isActive is truthy, the rendered HTML will be:

<p class="foo bar active">Hi</p>

If your component has multiple root elements, you would need to define which component will receive this class. You can do this using $attrs component property:

<div id="app">

  <my-component class="baz"></my-component>

</div>

const app = Vue.createApp({})

app.component('my-component', {

  template: `

    <p :class="$attrs.class">Hi!</p>

    <span>This is a child component</span>

  `

})

You can learn more about component attribute inheritance in the Non-Prop[ Attributes](https://v3.vuejs.org/guide/component-attrs.html) section.

<h3 id="#binding-inline-styles">
[#](https://v3.vuejs.org/guide/class-and-style.html#binding-inline-styles)Binding Inline Styles</h3>


<h4 id="#object-syntax">
[#](https://v3.vuejs.org/guide/class-and-style.html#object-syntax-2)Object Syntax</h4>


The object syntax for :style is pretty straightforward - it looks almost like CSS, except it's a JavaScript object. You can use either camelCase or kebab-case (use quotes with kebab-case) for the CSS property names:

<div :style="{ color: activeColor, fontSize: fontSize + 'px' }"></div>

data() {

  return {

    activeColor: 'red',

    fontSize: 30

  }

}

It is often a good idea to bind to a style object directly so that the template is cleaner:

<div :style="styleObject"></div>

data() {

  return {

    styleObject: {

      color: 'red',

      fontSize: '13px'

    }

  }

}

Again, the object syntax is often used in conjunction with computed properties that return objects.

<h4 id="#array-syntax">
[#](https://v3.vuejs.org/guide/class-and-style.html#array-syntax-2)Array Syntax</h4>


The array syntax for :style allows you to apply multiple style objects to the same element:

<div :style="[baseStyles, overridingStyles]"></div>

<h4 id="#auto-prefixing">
[#](https://v3.vuejs.org/guide/class-and-style.html#auto-prefixing)Auto-prefixing</h4>


When you use a CSS property that requires [vendor prefixes ](https://developer.mozilla.org/en-US/docs/Glossary/Vendor_Prefix)

in :style, for example transform, Vue will automatically detect and add appropriate prefixes to the applied styles.

<h4 id="#multiple-values">
[#](https://v3.vuejs.org/guide/class-and-style.html#multiple-values)Multiple Values</h4>


You can provide an array of multiple (prefixed) values to a style property, for example:

<div :style="{ display: ['-webkit-box', '-ms-flexbox', 'flex'] }"></div>

This will only render the last value in the array which the browser supports. In this example, it will render display: flex for browsers that support the unprefixed version of flexbox.

<h2 id="conditional-rendering">Conditional Rendering</h2>


<h3 id="#v-if">
[#](https://v3.vuejs.org/guide/conditional.html#v-if)v-if</h3>


The directive v-if is used to conditionally render a block. The block will only be rendered if the directive's expression returns a truthy value.

<h1 v-if="awesome">Vue is awesome!</h1>

It is also possible to add an "else block" with v-else:

<h1 v-if="awesome">Vue is awesome!</h1>

<h1 v-else>Oh no 😢</h1>

<h4 id="#conditional-groups-with-v-if-on-<template>">
[#](https://v3.vuejs.org/guide/conditional.html#conditional-groups-with-v-if-on-template)Conditional Groups with v-if on <template></h4>


Because v-if is a directive, it has to be attached to a single element. But what if we want to toggle more than one element? In this case we can use v-if on a <template> element, which serves as an invisible wrapper. The final rendered result will not include the <template> element.

<template v-if="ok">

  <h1>Title</h1>

  <p>Paragraph 1</p>

  <p>Paragraph 2</p>

</template>

<h4 id="#v-else">
[#](https://v3.vuejs.org/guide/conditional.html#v-else)v-else</h4>


You can use the v-else directive to indicate an "else block" for v-if:

<div v-if="Math.random() > 0.5">

  Now you see me

</div>

<div v-else>

  Now you don't

</div>

A v-else element must immediately follow a v-if or a v-else-if element - otherwise it will not be recognized.

<h4 id="#v-else-if">
[#](https://v3.vuejs.org/guide/conditional.html#v-else-if)v-else-if</h4>


The v-else-if, as the name suggests, serves as an "else if block" for v-if. It can also be chained multiple times:

<div v-if="type === 'A'">

  A

</div>

<div v-else-if="type === 'B'">

  B

</div>

<div v-else-if="type === 'C'">

  C

</div>

<div v-else>

  Not A/B/C

</div>

Similar to v-else, a v-else-if element must immediately follow a v-if or a v-else-if element.

<h3 id="#v-show">
[#](https://v3.vuejs.org/guide/conditional.html#v-show)v-show</h3>


Another option for conditionally displaying an element is the v-show directive. The usage is largely the same:

<h1 v-show="ok">Hello!</h1>

The difference is that an element with v-show will always be rendered and remain in the DOM; v-show only toggles the display CSS property of the element.

v-show doesn't support the <template> element, nor does it work with v-else.

<h3 id="#v-if-vs-v-show">
[#](https://v3.vuejs.org/guide/conditional.html#v-if-vs-v-show)v-if vs v-show</h3>


v-if is "real" conditional rendering because it ensures that event listeners and child components inside the conditional block are properly destroyed and re-created during toggles.

v-if is also lazy: if the condition is false on initial render, it will not do anything - the conditional block won't be rendered until the condition becomes true for the first time.

In comparison, v-show is much simpler - the element is always rendered regardless of initial condition, with CSS-based toggling.

Generally speaking, v-if has higher toggle costs while v-show has higher initial render costs. So prefer v-show if you need to toggle something very often, and prefer v-if if the condition is unlikely to change at runtime.

<h3 id="#v-if-with-v-for">[#](https://v3.vuejs.org/guide/conditional.html#v-if-with-v-for)v-if with v-for</h3>


Note

Using v-if and v-for together is not recommended. See the [style guide](https://v3.vuejs.org/style-guide/#avoid-v-if-with-v-for-essential) for further information.

When v-if and v-for are both used on the same element, v-if will be evaluated first. See the [list rendering guide](https://v3.vuejs.org/guide/list#v-for-with-v-if) for details.

<h2 id="list-rendering">List Rendering</h2>


<h3 id="#mapping-an-array-to-elements-with-v-for">
[#](https://v3.vuejs.org/guide/list.html#mapping-an-array-to-elements-with-v-for)Mapping an Array to Elements with v-for</h3>


We can use the v-for directive to render a list of items based on an array. The v-for directive requires a special syntax in the form of item in items, where items is the source data array and item is an alias for the array element being iterated on:

<ul id="array-rendering">

  <li v-for="item in items">

    {{ item.message }}

  </li>

</ul>

Vue.createApp({

  data() {

    return {

      items: [{ message: 'Foo' }, { message: 'Bar' }]

    }

  }

}).mount('#array-rendering')

Result:

Inside v-for blocks we have full access to parent scope properties. v-for also supports an optional second argument for the index of the current item.

<ul id="array-with-index">

  <li v-for="(item, index) in items">

    {{ parentMessage }} - {{ index }} - {{ item.message }}

  </li>

</ul>

Vue.createApp({

  data() {

    return {

      parentMessage: 'Parent',

      items: [{ message: 'Foo' }, { message: 'Bar' }]

    }

  }

}).mount('#array-with-index')

Result:

You can also use of as the delimiter instead of in, so that it is closer to JavaScript's syntax for iterators:

<div v-for="item of items"></div>

<h3 id="#v-for-with-an-object">
[#](https://v3.vuejs.org/guide/list.html#v-for-with-an-object)v-for with an Object</h3>


You can also use v-for to iterate through the properties of an object.

<ul id="v-for-object" class="demo">

  <li v-for="value in myObject">

    {{ value }}

  </li>

</ul>

Vue.createApp({

  data() {

    return {

      myObject: {

        title: 'How to do lists in Vue',

        author: 'Jane Doe',

        publishedAt: '2016-04-10'

      }

    }

  }

}).mount('#v-for-object')

Result:

You can also provide a second argument for the property's name (a.k.a. key):

<li v-for="(value, name) in myObject">

  {{ name }}: {{ value }}

</li>

And another for the index:

<li v-for="(value, name, index) in myObject">

  {{ index }}. {{ name }}: {{ value }}

</li>

Note

When iterating over an object, the order is based on the enumeration order of Object.keys(), which isn't guaranteed to be consistent across JavaScript engine implementations.

<h3 id="#maintaining-state">
[#](https://v3.vuejs.org/guide/list.html#maintaining-state)Maintaining State</h3>


When Vue is updating a list of elements rendered with v-for, by default it uses an "in-place patch" strategy. If the order of the data items has changed, instead of moving the DOM elements to match the order of the items, Vue will patch each element in-place and make sure it reflects what should be rendered at that particular index.

This default mode is efficient, but only suitable when your list render output does not rely on child component state or temporary DOM state (e.g. form input values).

To give Vue a hint so that it can track each node's identity, and thus reuse and reorder existing elements, you need to provide a unique key attribute for each item:

<div v-for="item in items" :key="item.id">

  <!-- content -->

</div>

It is recommended to provide a key attribute with v-for whenever possible, unless the iterated DOM content is simple, or you are intentionally relying on the default behavior for performance gains.

Since it's a generic mechanism for Vue to identify nodes, the key also has other uses that are not specifically tied to v-for, as we will see later in the guide.

Note

Don't use non-primitive values like objects and arrays as v-for keys. Use string or numeric values instead.

For detailed usage of the key attribute, please see the [key API documentation](https://v3.vuejs.org/api/special-attributes.html#key).

<h3 id="#array-change-detection">
[#](https://v3.vuejs.org/guide/list.html#array-change-detection)Array Change Detection</h3>


<h4 id="#mutation-methods">
[#](https://v3.vuejs.org/guide/list.html#mutation-methods)Mutation Methods</h4>


Vue wraps an observed array's mutation methods so they will also trigger view updates. The wrapped methods are:



*   push()
*   pop()
*   shift()
*   unshift()
*   splice()
*   sort()
*   reverse()

You can open the console and play with the previous examples' items array by calling their mutation methods. For example: example1.items.push({ message: 'Baz' }).

<h4 id="#replacing-an-array">
[#](https://v3.vuejs.org/guide/list.html#replacing-an-array)Replacing an Array</h4>


Mutation methods, as the name suggests, mutate the original array they are called on. In comparison, there are also non-mutating methods, e.g. filter(), concat() and slice(), which do not mutate the original array but always return a new array. When working with non-mutating methods, you can replace the old array with the new one:

example1.items = example1.items.filter(item => item.message.match(/Foo/))1

You might think this will cause Vue to throw away the existing DOM and re-render the entire list - luckily, that is not the case. Vue implements some smart heuristics to maximize DOM element reuse, so replacing an array with another array containing overlapping objects is a very efficient operation.

<h3 id="#displaying-filtered-sorted-results">
[#](https://v3.vuejs.org/guide/list.html#displaying-filtered-sorted-results)Displaying Filtered/Sorted Results</h3>


Sometimes we want to display a filtered or sorted version of an array without actually mutating or resetting the original data. In this case, you can create a computed property that returns the filtered or sorted array.

For example:

<li v-for="n in evenNumbers" :key="n">{{ n }}</li>

data() {

  return {

    numbers: [ 1, 2, 3, 4, 5 ]

  }

},

computed: {

  evenNumbers() {

    return this.numbers.filter(number => number % 2 === 0)

  }

}

In situations where computed properties are not feasible (e.g. inside nested v-for loops), you can use a method:

<ul v-for="numbers in sets">

  <li v-for="n in even(numbers)" :key="n">{{ n }}</li>

</ul>

data() {

  return {

    sets: [[ 1, 2, 3, 4, 5 ], [6, 7, 8, 9, 10]]

  }

},

methods: {

  even(numbers) {

    return numbers.filter(number => number % 2 === 0)

  }

}

<h3 id="#v-for-with-a-range">
[#](https://v3.vuejs.org/guide/list.html#v-for-with-a-range)v-for with a Range</h3>


v-for can also take an integer. In this case it will repeat the template that many times.

<div id="range" class="demo">

  <span v-for="n in 10" :key="n">{{ n }} </span>

</div>

Result:

<h3 id="#v-for-on-a-<template>">
[#](https://v3.vuejs.org/guide/list.html#v-for-on-a-template)v-for on a <template></h3>


Similar to template v-if, you can also use a <template> tag with v-for to render a block of multiple elements. For example:

<ul>

  <template v-for="item in items" :key="item.msg">

    <li>{{ item.msg }}</li>

    <li class="divider" role="presentation"></li>

  </template>

</ul>

<h3 id="#v-for-with-v-if">
[#](https://v3.vuejs.org/guide/list.html#v-for-with-v-if)v-for with v-if</h3>


TIP

Note that it's not recommended to use v-if and v-for together. Refer to the style[ guide](https://v3.vuejs.org/style-guide/#avoid-v-if-with-v-for-essential) for details.

When they exist on the same node, v-if has a higher priority than v-for. That means the v-if condition will not have access to variables from the scope of the v-for:

<!-- This will throw an error because property "todo" is not defined on instance. -->

<li v-for="todo in todos" v-if="!todo.isComplete">

  {{ todo.name }}

</li>

This can be fixed by moving v-for to a wrapping <template> tag:

<template v-for="todo in todos" :key="todo.name">

  <li v-if="!todo.isComplete">

    {{ todo.name }}

  </li>

</template>

<h3 id="#v-for-with-a-component">
[#](https://v3.vuejs.org/guide/list.html#v-for-with-a-component)v-for with a Component</h3>


This section assumes knowledge of [Components](https://v3.vuejs.org/guide/component-basics.html). Feel free to skip it and come back later.

You can directly use v-for on a custom component, like any normal element:

<my-component v-for="item in items" :key="item.id"></my-component>

However, this won't automatically pass any data to the component, because components have isolated scopes of their own. In order to pass the iterated data into the component, we should also use props:

<my-component

  v-for="(item, index) in items"


<p id="gdcalert2" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert3">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


  :item="item"


<p id="gdcalert3" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert4">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


  :index="index"


<p id="gdcalert4" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert5">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


  :key="item.id"

></my-component>

The reason for not automatically injecting item into the component is because that makes the component tightly coupled to how v-for works. Being explicit about where its data comes from makes the component reusable in other situations.

Here's a complete example of a simple todo list:

<div id="todo-list-example">

  <form v-on:submit.prevent="addNewTodo">

    <label for="new-todo">Add a todo</label>

    <input

      v-model="newTodoText"

      id="new-todo"

      placeholder="E.g. Feed the cat"

    />

    <button>Add</button>

  </form>

  <ul>

    <todo-item

      v-for="(todo, index) in todos"


<p id="gdcalert5" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert6">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


      :key="todo.id"


<p id="gdcalert6" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: Definition &darr;&darr; outside of definition list. Missing preceding term(s)? </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert7">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


      :title="todo.title"

      @remove="todos.splice(index, 1)"

    ></todo-item>

  </ul>

</div>

const app = Vue.createApp({

  data() {

    return {

      newTodoText: '',

      todos: [

        {

          id: 1,

          title: 'Do the dishes'

        },

        {

          id: 2,

          title: 'Take out the trash'

        },

        {

          id: 3,

          title: 'Mow the lawn'

        }

      ],

      nextTodoId: 4

    }

  },

  methods: {

    addNewTodo() {

      this.todos.push({

        id: this.nextTodoId++,

        title: this.newTodoText

      })

      this.newTodoText = ''

    }

  }

})

app.component('todo-item', {

  template: `

    <li>

      {{ title }}

      <button @click="$emit('remove')">Remove</button>

    </li>

  `,

  props: ['title'],

  emits: ['remove']

})

app.mount('#todo-list-example')

<h2 id="main-files">Main Files</h2>


<h3 id="app-vue">App.vue</h3>


App.vue is a Single File Component and is a great way to create self-contained components that have all they need in a single file. We have the markup, the JavaScript that is going to interact with it, and style that’s applied to it, which can be scoped, or not. In this case, it’s not scoped, and it’s just outputting that CSS which is applied like regular CSS to the page. The interesting part lies in the script tag where all relevant components are declared as a dependency.

When a Vue instance is created, it adds all the properties found in its data object to Vue’s reactivity system. When the values of those properties change, the view will “react”, updating to match the new values. When << data >> changes, the view will re-render. It should be noted that properties in data are only reactive if they existed when the instance was created.

VBUS - custom event bus for letting unrelated components talk to each other. Initialize Top bar, footer, relevant theme scss file and relevant styling class(es)

<h3 id="miniwin-vue">Miniwin.vue</h3>


All key components along with agrs & necessary transitions to form a Mini Window for Projects Platform. It is one the key components along with TopBar, Big Window, Application Dialog, Popup & Message components to show the information and preview Project data.

<h3 id="msg-vue">Msg.vue</h3>


Leverage UserCard for displaying messages of the passed argument with appropriate transitions.

<h3 id="bigwin-vue">BigWin.vue</h3>


We can use the v-on directive to listen to DOM events and run some JavaScript when they’re triggered. Detects the mode in which the Projects platform is being utilized.

<h3 id="topbar-vue">**TopBar.vue**</h3>


TopBar components with the relevant logo information (based on organizations) along with portal language, search portal button with material icons for small display sizes, online help documentation along with project category icon. Google login button redirects them to keycloak login, logout windows based on user authentication status. The TopBar is a shared component that includes organization brand collaterals (conditional logo & branding), portal language (currently English, French & Simplified Chinese), search (currently database search not elastic search), contextual help (end user documentation) and user’s profile avatar and name(if user is logged in).



<p id="gdcalert7" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image1.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert8">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image1.png "image_tooltip")


<h3 id="main-css">**Main.css**</h3>


Key CSS file for #APP and other key views stylings.

<h3 id="main-js">**Main.js**</h3>


Key js consequential file where the Projects platform starts. The external libraries like JQuery, Leaflet, Bulma, Axios etc. are imported in main.js. This is where the global inter component communication bus **VBUS** is initialized along with pre-configuring Axios according to the organization id . 

Computed properties let perform complex operations or data formatting while maximizing performance with dependency calculations that only update the view when a dependency changes. This feature is synchronous. However, we leverage the _vue-async-computed_ package to create and consume asynchronous computed properties in projects’ components by binding the resolved value of a Promise to a component property. 

The **Translate** function uses Translate JSON file to make Projects platform multilingual to include multiple labels in multiple languages to be swapped on user selection. The toHtmlTB function makes addition or deletion of language(s) easy & modular. 

This is the file that initializes export of Global Shared Object (GS) as a substitute for state handling external libraries like Vuex. The object seeds the categories according to the organizations along with the API data properties linked to the user(people) and the organization. We use **[URLSearchParams](https://developer.mozilla.org/en-US/docs/Web/API/URLSearchParams)** to define utility methods to work with the query string of a URL. GS object implementing URLSearchParams can directly be used in a “for...of” structure that allows us to manipulate the state and check connection by returning the first value associated with the given search parameter and allowing iteration through all keys of the key/value pairs contained in this object. Key point to note is that URLSearchParams constructor does not parse full URLs. However, it will strip an initial leading ? off of a string, if present.

The **history**.**replaceState**() method modifies the current history entry, replacing it with the stateObj, title, and URL passed in the method parameters. This method is particularly useful when you want to update the state object or URL of the current history entry in response to some user action.



<p id="gdcalert8" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image2.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert9">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image2.png "image_tooltip")


We leverage AXIOS post to send bearer tokens where the first parameter is the URL. The second is the JSON body that will be sent along the request. The third parameter are the headers (among other things), which is JSON as well. 



<p id="gdcalert9" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image3.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert10">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image3.png "image_tooltip")


The same helps ascertain users authorization levels and check the connection loop to initialize Projects Platform in the right state based on user’s authorization & authentication level. Projects Platform application uses function **initProjects**() to configure all the global Axios defaults. [Axios interceptors](https://github.com/axios/axios#interceptors) intercept requests or responses before they are handled by then or catch. The interceptors are used to append every request with XSRF tokens for security and to catch all global errors and return AMIGA guru meditation errors(What!!!) linked with 401, 403, 417, 422, 501 error codes.  Key thing to note is that the request interceptors are presumed to be asynchronous by default. This can cause a delay in the execution of the axios request when the main thread is blocked (a promise is created under the hood for the interceptor and the request gets put on the bottom of the call stack). If request interceptors are synchronous we could add a flag to the options object that will tell axios to run the code synchronously and avoid any delays in request execution. The initialize function sets the current theme, portal language and relevant organization parameters including main categories, stylings.

<h3 id="router-js">**Router.js**</h3>


Router file leverages Vue Router to put all the Projects platform components in hierarchy explicitly mentioning child parent relationships (route nesting). The key part to focus on in this file is that the routes of our Vue app are defined via an array that contains objects. Each route object contains three key properties: 



*   Path - what URL should match to the component. 
*   Name - what this route should be named for labeling and debugging purposes. 
*   Component - the component that should be displayed when the path is matched. 


```
routes: [
   {
     path: '/',
     name: 'Home',
     component: pageHome
   },
   {
     path: '/logout',
     beforeEnter() { location.href = GS.apisrv+'/logout?home='+  btoa(window.location.origin) }
   },
   {
     path: '/me',
     name: 'myhomepage',
     component: pageMe,
     children: [
       { path: 'followed',
         name: "followed",
         component: subMeFollowed,
       },
       { path: 'myprojects',
         name: "myprojects",
         component: subMeMyProjects,
       },
       { path: 'toreview',
         name: "toreview",
         component: subMeReviewed,
       },
     ]
   },
   {
     path: '/admin',
     name: 'Admin',
     component: pageAdmin,
     children: [
       { path: 'portal',
         name: "portal",
         component: PortalAdmin,
         children: [
           {
             path: 'general',
             name: "general",
             component: PortalGeneralAdmin,
           },
           {
             path: 'concepts',
             name: "concepts",
             component: ConceptsAdmin,
           },
           {
             path: 'types',
             name: "types",
             component: TypesAdmin,
           }
         ]
       },
       { path: 'contents',
         name: "contents",
         component: ContentAdmin,
       },
       { path: 'users',
         name: "users",
         component: UserAdmin,
       }
     ]
   },
   {
     path: '/repo/',
     name: 'type',
     component: pageCat,
     props: true
   },
   {
     path: '/repo/:type',
     name: 'type',
     component: pageCat,
     props: true
   },
   {
     path: '/projects',
     name: 'projects',
     component: pageBrowse,
   },
   {
     path: '/map',
     name: 'map',
     component: pageMap,
   },
   {
     path: '/concepts-map',
     name: 'concepts-map',
     component: ConceptsMap
   },
   {
     path: '/projects/:id',
     name: 'pageproject',
     component: pageProject,
     children: [
       { path: 'summary',
         name: "projectsummary",
         component: subProjectSummary,
       },
       { path: 'des',
         name: "projectdes",
         component: subProjectDes,
       },
       { path: 'blogentries',
         name: "projectblog",
         component: subProjectBlog,
       },
       { path: 'goals',
         name: "projectgoals",
         component: subProjectGoals,
       },
       { path: 'team',
         name: "projectteam",
         component: subProjectTeam,
       },
       { path: 'ressources',
         name: "projectressources",
         component: subProjectRes,
       },
       { path: 'comments',
         name: "projectcomments",
         component: subProjectComments,
       },
     ]
   },
   {
     path: '/editproject/:id',
     component: pageEditProject,
     children: [
       { path: 'general',
         name: "editproject",
         component: subEditProjectGen,
       },
     ]
   },
   {
     path: '/stats',
     name: "stat",
     component: Stat
   }
 ]
})
```


<h3 id="appdialog-vue">**AppDialog.vue**</h3>


Parent component of Gallery & Video provider chooser components that allows inclusion of Image gallery & Video embed components.

<h3 id="popup-vue">**PopUp.vue**</h3>


Parent component for Error, Info & Progress components with mode & arguments as props with relevant transitions.

<h2 id="shared-components">Shared Components</h2>


<h4 id="admin-sidebar">Admin Sidebar</h4>


<h5 id="admin-routes-js">Admin Routes (js)</h5>


<h5 id="admin-sidebar-vue">Admin Sidebar (vue)</h5>


<h5 id="menu-item-vue">Menu Item (vue)</h5>


<h2 id="functions">Functions</h2>


<h4 id="api">API</h4>


<h4 id="organizations-services-js">Organizations Services (js)</h4>


Specific file for retrieving & updating leveraging AXIOS Get & Patch operations. The filter for fetching organisations according to concepts and using getAxiosConfig with etag token for updating respective organizations passing the formData as an argument from the Portal general Admin component.  

<h4 id="types-services-js">Types Services (js)</h4>


Specialized file for projects' types that helps projects platform users thematically differentiate the projects. There CRUD operations around the project types that are synchronous(mainly get(getType) and filter operations by respective organizations(getTypesByOrg)) or asynchronous leveraging Axios post(addType), patch(updateType), delete(deleteType).

<h4 id="api-services-js">API services (js)</h4>


Central definition for all the relevant functions that are utilized across the Projects platform code including Image upload, file upload, search in PeopleAPI, get specific user, wiki concepts (category) & project, publish projects, project CRUD dispositions, project categories, blog entries, SDGs, 3rd party resources, project reviews & comments, organization(s) and make GET, POST, PATCH, DELETE request(s) using Axios to get, push, patch, post and delete data to/from a given endpoint and trigger events.

Imports Global shared(GS) object and utilizes a 3rd party library like Axios that is an HTTP client library which uses promises by default and runs on both the client and the server, which makes it appropriate for fetching data during server-side rendering. Because it uses promises, we combine it with async/await to get a concise and easy-to-use API. 

<h4 id="constants-js">Constants (js)</h4>


Declare constants in a separate constants.js file which we can require into the other Vue component:



*   Sustainable Development Goals(SDG) Codes
*   SDG labels
*   SDG Colors
*   Months
*   Media file Upload Constraints

<h4 id="dotatlas-js">Dotatlas (js)</h4>


dotAtlas is a JavaScript library for interactive exploration of 2d point collections. dotAtlas can produce zoomable visualizations similar to the one shown below. They combine various types of layers, such as elevations, markers or labels, to produce an attractive map-like presentation of your data.



<p id="gdcalert10" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image4.jpg). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert11">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image4.jpg "image_tooltip")




---


dotAtlas, in essence, is a map-like visualization of 2d points for browsers. 



*   Customizable colors, sizes, shapes, opacities, elevations and textual labels for all the points.
*   Independent control of the elevations, markers, outline and label layers.
*   Built-in finding clusters of nearby points for easy multi-point hover and selection.
*   WebGL-based implementation for 60 FPS interaction animations, also with large data sets.

There are three ways to get started with dotAtlas:



*   [Quick start](https://get.carrotsearch.com/dotatlas/latest/doc/quick-start/): setting up your first simple dotAtlas visualization with a minimal amount of code.
*   Guides: in-depth articles covering various aspects of dotAtlas, such as [requirements](https://get.carrotsearch.com/dotatlas/latest/doc/requirements/), [installation](https://get.carrotsearch.com/dotatlas/latest/doc/installation/), [API overview](https://get.carrotsearch.com/dotatlas/latest/doc/api-overview/), [defining layers](https://get.carrotsearch.com/dotatlas/latest/doc/defining-layers/), [listening to events](https://get.carrotsearch.com/dotatlas/latest/doc/listening-to-events/) and more.
*   [Tutorial](https://get.carrotsearch.com/dotatlas/latest/doc/tutorial/): step by step instructions on building a more complex dotAtlas visualization, including: layer set-up, handling user interactions and implementing hover and selection highlights.

Finally, the [API](https://get.carrotsearch.com/dotatlas/latest/doc/api-common/) [references](https://get.carrotsearch.com/dotatlas/latest/doc/api-dotatlas/) contain details on all the available options and methods.

<h4 id="functions-js">Functions (js)</h4>


Key functions that export the authorization and authentication of the user and provide appropriate privileges including project edit, publish & review rights to the user and relevant project(s). Key functions to copy objects simply, user authentication & authorization with regards to the Project resources, check email; URL validity etc. 

<h2 id="pages">Pages</h2>


<h3 id="admin-pages">Admin Pages</h3>


<h3 id="sub-pages-components">Sub Pages - Components</h3>


<h3 id="main-pages-components">Main Pages - Components</h3>


<h2 id="window-components">Window Components</h2>


<h3 id="application-dialogs">Application Dialogs</h3>


<h4 id="gallery-vue">Gallery.vue</h4>


Dedicated component uploading images to the project from the local system and prompts warning text when there aren’t any images linked with the project. The component methods include add images, select images, insert images, cancel select images, get image details, load images, delete images with relevant transitions. Load Images (loadImagesPrevNext) leverages Axios GET to immediately send requests to the server including image meta information.  



<p id="gdcalert11" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image5.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert12">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image5.png "image_tooltip")


<h4 id="videoproviderchooser-vue">VideoProviderChooser.vue</h4>


Dedicated component to choose videos to the project from the local system and prompts warning text when there aren’t any images linked with the project. The component methods include validate video links, add video, add images, select video, insert videos, cancel select, get video details, load video, delete video with relevant transitions. Validate video links (validateVideoLink) leverages Axios GET to immediately send requests to the server including links meta information. The function checks the URL validity if the whole URL gets entered or just the shortid of Vimeo or YouTube.



<p id="gdcalert12" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image6.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert13">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image6.png "image_tooltip")


<h3 id="mini-windows">Mini Windows</h3>


<h4 id="copy-vue">Copy.vue</h4>


Specific component for copying resources & cancel using copyObj and runCB methods emitting mini window through custom event bus (VBUS).



<p id="gdcalert13" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image7.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert14">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image7.png "image_tooltip")


<h4 id="copylink-vue">CopyLink.vue</h4>


The component that is used in the Project Blog component to copy the link of an added blog entry for easy sharing. The same leverages Props argument to get event & linkid from ProjectBlog.vue to construct the URL(makelink) in format: window.location.origin + "/projects/" + GS.currentprojectid +"/blogentries?b="+self.args.linkid (e.g. [https://dev.cri-paris.org:43103/projects/VCstJe3S/blogentries?b=603f5697cfd658c33a1b5d51](https://dev.cri-paris.org:43103/projects/VCstJe3S/blogentries?b=603f5697cfd658c33a1b5d51))



<p id="gdcalert14" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image8.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert15">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image8.png "image_tooltip")


<h4 id="editresfile-vue">EditResFile.vue</h4>


Specific component to edit each of the file resources using patchRes method through custom event bus (VBUS). The component uses respatch function and passes current obj._id along with modified data to the api respatch function.

<h4>

<p id="gdcalert15" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image9.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert16">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image9.png "image_tooltip")
</h4>


<h4 id="edit-reslink-vue">Edit ResLink.vue</h4>


Specific component to edit each of the URL link  resources using patchRes method through custom event bus (VBUS). The component uses respatch function and passes current obj._id,  along with modified data to the api respatch function. The component loops through link categories (resource categories) from the constants file.



<p id="gdcalert16" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image10.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert17">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image10.png "image_tooltip")


<h4 id="editresproject-vue">EditResProject.vue</h4>


Specific component for the mini window to edit each of the Project resources using patchRes method through custom event bus (VBUS). The component uses respatch function and passes current obj._id,  along with modified data to the api respatch function. The component loops through link categories along with project categories (resource categories from English & French) from the constants file. The same also includes TextInput from shared components to allow the user to annotate the link reason.



<p id="gdcalert17" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image11.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert18">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image11.png "image_tooltip")


<h4 id="miniinfo-vue">MiniInfo.vue</h4>


Specific component for passing content title & description as argument content’s title & description to Mini window component.

<h6>

<p id="gdcalert18" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image12.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert19">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image12.png "image_tooltip")
</h6>


<h4 id="unsaveddata-vue">UnsavedData.vue</h4>


Specific component for confirming unsaved data of resource using runCB methods emitting mini window close through custom event bus (VBUS).

<h4 id="yesno-vue">YesNo.vue</h4>


Specific component for confirming deletion of resource using runCB methods emitting mini window close through custom event bus (VBUS).



<p id="gdcalert19" ><span style="color: red; font-weight: bold">>>>>>  gd2md-html alert: inline image link here (to images/image13.png). Store image on your image server and adjust path/filename/extension if necessary. </span><br>(<a href="#">Back to top</a>)(<a href="#gdcalert20">Next alert</a>)<br><span style="color: red; font-weight: bold">>>>>> </span></p>


![alt_text](images/image13.png "image_tooltip")


<h3 id="popup-windows">Popup Windows</h3>


<h2 id="translation-files">Translation Files</h2>


<h2 id="routing">Routing</h2>


<h2 id="transitions-&-animations">Transitions & Animations</h2>


<h2 id="external-libraries">External Libraries</h2>


<h4 id="vue-js">Vue.js</h4>


[Vue.js](https://vuejs.org/) is a javascript web framework. 

<h4 id="tiptap">TipTap</h4>


[TipTap](https://github.com/ueberdosis/tiptap) is a toolkit for building text editors. We are using the vue package for TipTap. TipTap is an extension to [ProseMirror](https://prosemirror.net/) that allows you to create new schemas directly in a vue way. 

This editor is used to edit a project's description or blog post.

<h4 id="vue-leaflet">Vue Leaflet</h4>


[Vue Leaflet](https://vue2-leaflet.netlify.app/) is a vue package built on Leaflet. 

Leaflet is a strong package to build maps and interact with it.

<h4 id="vue-color">Vue Color</h4>


[Vue Color](https://github.com/xiaokaike/vue-color) is a vue color picker package. It provides a different picker from simple hex code to color choice with opacity. 

We are using it to let organization administrators select a background color for categories.

<h4 id="axios">Axios</h4>


[Axios](https://github.com/axios/axios) is an Http client. 

We are using it to manage HTTP calls to our API. It is based on promise.

<h4 id="drag-and-resize">Drag and resize</h4>


[vue-drag-resize](https://github.com/kirillmurashov/vue-drag-resize) is a package made for image resizing and dragging. 

We are using it on blog post and description when user upload images or videos

<h4 id="bulma">Bulma</h4>


[Bulma](https://bulma.io/) is a CSS framework. We are using the basic version for responsibility and basic component class : Button, Grid etc. 

We are also using some components of [Bulma extension](https://bulma.io/extensions/) that bring css/js components like tooltip.

<h4 id="chartjs">ChartJs</h4>


[vue-chartjs](https://vue-chartjs.org/) is a vue wrapper to Chart.js 

We are using it to build chart in Stats page

<h2 id="state-management">State Management</h2>


<h2 id="server-side-rendering">Server side Rendering</h2>


<h2 id="backend-apis">Backend APIs</h2>


<h4>### api </h4>


APIs are registered here. Eve hooks and initialisation. 

<h4>### Authentication </h4>


Endpoints about authentication are in `api_auth.py`. 2 authentication was available : CRIID and OPENID. CRIIS is legacy and only OPENID should be used. It should be move in /auth folder 

<h4>### api_cstm </h4>


This file contains all endpoints that are not handled by Eve. Those endpoints are built with Flask and the required package depends on what the service needs to do. 

<h4 id="###-api_funct">### api_funct</h4>


api_funct_sec, api_funct_mail, api_funct_db Tools function. It would be a good idea to create a tools folder and put those file with a better naming 

<h4>### api_private </h4>


Endpoints for server authentication or IP restricted. Used for internal apps communication or client that need to consume data (eg. Organizations) 

<h4>### ref </h4>


Reference API. Built to generate accessible projects pages for scrapping (like a custom Server-side-rendering). It will generate meta and project's images. 

<h4>### settings </h4>


Eve configuration file. DB model are represent here with schema and allowed HTTP VERB 

<h4>### migrations </h4>


It should contain all DB and file migration. Naming must be link to the version where the migration is needed (eg. v0.3.1) 

<h4>### exceptions </h4>


It should contains python specific exceptions we create 

<h4>### TPL </h4>


Should contain a flask template. There are used mainly for emails

-------------------------
