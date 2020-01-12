# jmeter-sc
# Script is created with jmeter 5.1.1 version
# Stepping Thread group is used to gradully increase concurrent threads. By defaut, jmeter don't have jp@gc-Stepping Thread Group, users have to add "JMeterPlugins-Standard"& "JMeterPlugins-Extras" in 'lib/ext' folder of jmeter.
# As all assertions are same due to same response available on 'http://dummy.restapiexample.com/", so I have added assertions globally (not for individual sampler)to avoid repitition.
But it can be added at sampler level as per responses in real world scenarios.
# As requirement was specific to concurrent users and not hits per second or throughput required, there is no control over hits per second, but if required, can be controlled with throughput controller.
# Script is creating a user first and then it is extracting "id" from create response and same id is getting used in 'Retrieve', 'Update' and 'Delete' calls respectively.
