---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php


$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestBody = new BookingBusiness();
$requestBody->setEmail('admin@fabrikam.com');
$schedulingPolicy = new BookingSchedulingPolicy();
$schedulingPolicy->setTimeSlotInterval(new \DateInterval('PT60M'));
$schedulingPolicy->setMinimumLeadTime(new \DateInterval('P1D'));
$schedulingPolicy->setMaximumAdvance(new \DateInterval('P30D'));
$schedulingPolicy->setSendConfirmationsToOwner(true);
$schedulingPolicy->setAllowStaffSelection(true);
$requestBody->setSchedulingPolicy($schedulingPolicy);

$result = $graphServiceClient->bookingBusinesses()->byBookingBusinessId('bookingBusiness-id')->patch($requestBody)->wait();

```