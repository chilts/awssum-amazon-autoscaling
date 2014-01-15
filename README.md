# awssum-amazon-autoscaling #

This is an ```AwsSum``` plugin!

You'll need to add [awssum-amazon-autoscaling](https://github.com/awssum/awssum-amazon-autoscaling/) to your package.json
dependencies. Both [awssum](https://github.com/awssum/awssum/) and
[awssum-amazon](https://github.com/awssum/awssum-amazon/) are pulled in as peer dependencies.

## Example ##

Describe all your alarms:

```
var fmt = require('fmt');
var amazonAutoScaling = require('awssum-amazon-autoscaling');

var autoscaling = new amazonAutoScaling.AutoScaling({
    'accessKeyId'     : process.env.ACCESS_KEY_ID,
    'secretAccessKey' : process.env.SECRET_ACCESS_KEY,
    'region'          : amazonAutoScaling.US_EAST_1
});

autoscaling.DescribeAutoScalingGroups(function(err, data) {
    fmt.dump(err, 'err');
    fmt.dump(data, 'data');
});
```

## Operations ##

* CreateAutoScalingGroup

Docs: [CreateAutoScalingGroup on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_CreateAutoScalingGroup.html)

* CreateLaunchConfiguration

Docs: [CreateLaunchConfiguration on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_CreateLaunchConfiguration.html)

* CreateOrUpdateTags

Docs: [CreateOrUpdateTags on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_CreateOrUpdateTags.html)

* DeleteAutoScalingGroup

Docs: [DeleteAutoScalingGroup on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_DeleteAutoScalingGroup.html)

* DeleteLaunchConfiguration

Docs: [DeleteLaunchConfiguration on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_DeleteLaunchConfiguration.html)

* DeleteNotificationConfiguration

Docs: [DeleteNotificationConfiguration on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_DeleteNotificationConfiguration.html)

* DeletePolicy

Docs: [DeletePolicy on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_DeletePolicy.html)

* DeleteScheduledAction

Docs: [DeleteScheduledAction on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_DeleteScheduledAction.html)

* DeleteTags

Docs: [DeleteTags on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_DeleteTags.html)

* DescribeAdjustmentTypes

Docs: [DescribeAdjustmentTypes on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_DescribeAdjustmentTypes.html)

* DescribeAutoScalingGroups

Docs: [DescribeAutoScalingGroups on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_DescribeAutoScalingGroups.html)

* DescribeAutoScalingInstances

Docs: [DescribeAutoScalingInstances on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_DescribeAutoScalingInstances.html)

* DescribeAutoScalingNotificationTypes

Docs: [DescribeAutoScalingNotificationTypes on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_DescribeAutoScalingNotificationTypes.html)

* DescribeLaunchConfigurations

Docs: [DescribeLaunchConfigurations on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_DescribeLaunchConfigurations.html)

* DescribeMetricCollectionTypes

Docs: [DescribeMetricCollectionTypes on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_DescribeMetricCollectionTypes.html)

* DescribeNotificationConfigurations

Docs: [DescribeNotificationConfigurations on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_DescribeNotificationConfigurations.html)

* DescribePolicies

Docs: [DescribePolicies on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_DescribePolicies.html)

* DescribeScalingActivities

Docs: [DescribeScalingActivities on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_DescribeScalingActivities.html)

* DescribeScalingProcessTypes

Docs: [DescribeScalingProcessTypes on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_DescribeScalingProcessTypes.html)

* DescribeScheduledActions

Docs: [DescribeScheduledActions on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_DescribeScheduledActions.html)

* DescribeTags

Docs: [DescribeTags on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_DescribeTags.html)

* DisableMetricsCollection

Docs: [DisableMetricsCollection on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_DisableMetricsCollection.html)

* EnableMetricsCollection

Docs: [EnableMetricsCollection on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_EnableMetricsCollection.html)

* ExecutePolicy

Docs: [ExecutePolicy on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_ExecutePolicy.html)

* PutNotificationConfiguration

Docs: [PutNotificationConfiguration on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_PutNotificationConfiguration.html)

* PutScalingPolicy

Docs: [PutScalingPolicy on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_PutScalingPolicy.html)

* PutScheduledUpdateGroupAction

Docs: [PutScheduledUpdateGroupAction on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_PutScheduledUpdateGroupAction.html)

* ResumeProcesses

Docs: [ResumeProcesses on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_ResumeProcesses.html)

* SetDesiredCapacity

Docs: [SetDesiredCapacity on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_SetDesiredCapacity.html)

* SetInstanceHealth

Docs: [SetInstanceHealth on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_SetInstanceHealth.html)

* SuspendProcesses

Docs: [SuspendProcesses on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_SuspendProcesses.html)

* TerminateInstanceInAutoScalingGroup

Docs: [TerminateInstanceInAutoScalingGroup on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_SuspendProcesses.html)

* UpdateAutoScalingGroup

Docs: [UpdateAutoScalingGroup on AWS](http://docs.amazonwebservices.com/AutoScaling/latest/APIReference/API_UpdateAutoScalingGroup.html)

# Author #

Written by [Andrew Chilton](http://chilts.org/) - [Blog](http://chilts.org/blog/) -
[Twitter](https://twitter.com/andychilton).

# License #

* [Copyright 2011-2013 Apps Attic Ltd.  All rights reserved.](http://appsattic.mit-license.org/2011/)
* [Copyright 2013 Andrew Chilton.  All rights reserved.](http://chilts.mit-license.org/2013/)

(Ends)
