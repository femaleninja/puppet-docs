---
layout: default
built_from_commit: 28833b083d1ed4cd328af45fbe26cfa00679c6b3
title: 'Resource Type: mailalias'
canonical: "/puppet/latest/types/mailalias.html"
---

> **NOTE:** This page was generated from the Puppet source code on 2018-03-20 07:07:39 -0700

mailalias
-----

* [Attributes](#mailalias-attributes)
* [Providers](#mailalias-providers)

<h3 id="mailalias-description">Description</h3>

Creates an email alias in the local alias database.

<h3 id="mailalias-attributes">Attributes</h3>

<pre><code>mailalias { 'resource title':
  <a href="#mailalias-attribute-name">name</a>      =&gt; <em># <strong>(namevar)</strong> The alias...</em>
  <a href="#mailalias-attribute-ensure">ensure</a>    =&gt; <em># The basic property that the resource should be...</em>
  <a href="#mailalias-attribute-file">file</a>      =&gt; <em># A file containing the alias's contents.  The...</em>
  <a href="#mailalias-attribute-recipient">recipient</a> =&gt; <em># Where email should be sent.  Multiple values...</em>
  <a href="#mailalias-attribute-target">target</a>    =&gt; <em># The file in which to store the aliases.  Only...</em>
  # ...plus any applicable <a href="{{puppet}}/metaparameter.html">metaparameters</a>.
}</code></pre>

<h4 id="mailalias-attribute-name">name</h4>

_(**Namevar:** If omitted, this attribute's value defaults to the resource's title.)_

The alias name.

([↑ Back to mailalias attributes](#mailalias-attributes))

<h4 id="mailalias-attribute-ensure">ensure</h4>

_(**Property:** This attribute represents concrete state on the target system.)_

The basic property that the resource should be in.

Default: `present`

Allowed values:

* `present`
* `absent`

([↑ Back to mailalias attributes](#mailalias-attributes))

<h4 id="mailalias-attribute-file">file</h4>

_(**Property:** This attribute represents concrete state on the target system.)_

A file containing the alias's contents.  The file and the
recipient entries are mutually exclusive.

([↑ Back to mailalias attributes](#mailalias-attributes))

<h4 id="mailalias-attribute-recipient">recipient</h4>

_(**Property:** This attribute represents concrete state on the target system.)_

Where email should be sent.  Multiple values
should be specified as an array.  The file and the
recipient entries are mutually exclusive.

([↑ Back to mailalias attributes](#mailalias-attributes))

<h4 id="mailalias-attribute-target">target</h4>

_(**Property:** This attribute represents concrete state on the target system.)_

The file in which to store the aliases.  Only used by
those providers that write to disk.

([↑ Back to mailalias attributes](#mailalias-attributes))


<h3 id="mailalias-providers">Providers</h3>

<h4 id="mailalias-provider-aliases">aliases</h4>






> **NOTE:** This page was generated from the Puppet source code on 2018-03-20 07:07:39 -0700