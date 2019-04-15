# Oracle Export Plugin

[![cm-available](https://cdap-users.herokuapp.com/assets/cm-available.svg)](https://docs.cdap.io/cdap/current/en/integrations/cask-market.html)
![cdap-action](https://cdap-users.herokuapp.com/assets/cdap-action.svg)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
[![Join CDAP community](https://cdap-users.herokuapp.com/badge.svg?t=wrangler)](https://cdap-users.herokuapp.com?t=1)

Introduction
============

Oracle Export plugin is an action that can efficiently export data from Oracle to be used in CDAP pipelines.  Oracle includes command line tools to export data that can be utilized to perform this task.


Getting Started
===============

Prerequisites
-------------
CDAP version 3.5.x or higher.

Building Plugins
----------------
You get started with Oracle Export plugins by building directly from the latest source code::

  git clone https://github.com/hydrator/oracle-export-action.git
  cd oracle-export-plugins
  mvn clean package

After the build completes, you will have a JAR for each plugin under each
``<plugin-name>/target/`` directory.

Deploying Plugins
-----------------
You can deploy a plugin using the CDAP CLI::

  > load artifact <target/plugin-jar> config-file <resources/plugin-config>

  > load artifact target/oracle-export-plugins-<version>.jar \
         config-file target/oracle-export-plugins-<version>.json

You can build without running tests: ``mvn clean install -DskipTests``


Mailing Lists
-------------
CDAP User Group and Development Discussions:

- `cdap-user@googlegroups.com <https://groups.google.com/d/forum/cdap-user>`__

The *cdap-user* mailing list is primarily for users using the product to develop
applications or building plugins for appplications. You can expect questions from
users, release announcements, and any other discussions that we think will be helpful
to the users.

IRC Channel
-----------
CDAP IRC Channel: #cdap on irc.freenode.net


License and Trademarks
======================

Copyright © 2015-2019 Cask Data, Inc.

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this file except
in compliance with the License. You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the
License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND,
either express or implied. See the License for the specific language governing permissions
and limitations under the License.

Cask is a trademark of Cask Data, Inc. All rights reserved.

Apache, Apache HBase, and HBase are trademarks of The Apache Software Foundation. Used with
permission. No endorsement by The Apache Software Foundation is implied by the use of these marks.

.. |(Hydrator)| image:: http://cask.co/wp-content/uploads/hydrator_logo_cdap1.png
