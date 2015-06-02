###################
Arquillian Tutorial
###################

This tutorial is based on the online Getting started tutorial_ of the arquillian testing environment.
It was necessary to add the aquillian.xml configuration file to the Netbeans project in the proper path (src/test/resources/)::

<?xml version="1.0" encoding="UTF-8"?>
<arquillian xmlns="http://jboss.org/schema/arquillian" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://jboss.org/schema/arquillian http://www.jboss.org/schema/arquillian/arquillian_1_0.xsd">
<container qualifier="arquillian-glassfish-embedded" default="true">
<configuration>
<property name="bindHttpPort">9090</property>
</configuration>
</container>
</arquillian>

The entire pom.xml_ and the additional dependencies_ are also online.



.. _tutorial: http://arquillian.org/guides/getting_started_de/
.. _pom.xml: https://gist.github.com/mojavelinux/1263934
.. _dependencies: http://arquillian.org/modules/arquillian-glassfish-embedded-3.1-container-adapter/
