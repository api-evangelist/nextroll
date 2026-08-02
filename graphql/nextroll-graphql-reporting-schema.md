<a id="graphql-reporting-api-schema"></a>

# GraphQL Reporting API Schema

#### NOTE
You can browse the schema and experiment with building queries using the [GraphQL Reporting API console](https://app.adroll.com/reporting/graphiql).

## Objects

Objects represent a set of fields.

### List

- [`Ad`](#Ad)
- [`AdGroupData`](#AdGroupData)
- [`AdLabel`](#AdLabel)
- [`AdQuery`](#AdQuery)
- [`Adgroup`](#Adgroup)
- [`AdgroupGroupData`](#AdgroupGroupData)
- [`AdgroupQuery`](#AdgroupQuery)
- [`Advertisable`](#Advertisable)
- [`AdvertisableGroupData`](#AdvertisableGroupData)
- [`AdvertisableMetricResult`](#AdvertisableMetricResult)
- [`AdvertisableQuery`](#AdvertisableQuery)
- [`Audience`](#Audience)
- [`AudienceGroupData`](#AudienceGroupData)
- [`AudienceMetric`](#AudienceMetric)
- [`AudienceMetricResult`](#AudienceMetricResult)
- [`Automation`](#Automation)
- [`AutomationNode`](#AutomationNode)
- [`AutomationQuery`](#AutomationQuery)
- [`CTVPlacement`](#CTVPlacement)
- [`CTVPlacementResult`](#CTVPlacementResult)
- [`Campaign`](#Campaign)
- [`CampaignGroupData`](#CampaignGroupData)
- [`CampaignMetricResult`](#CampaignMetricResult)
- [`CampaignQuery`](#CampaignQuery)
- [`ContextualKeywordTargetingMetrics`](#ContextualKeywordTargetingMetrics)
- [`ContextualTargetingResult`](#ContextualTargetingResult)
- [`ContextualTopicTargetingMetrics`](#ContextualTopicTargetingMetrics)
- [`ConversionResult`](#ConversionResult)
- [`Conversions`](#Conversions)
- [`ConversionsByDate`](#ConversionsByDate)
- [`ConversionsSummary`](#ConversionsSummary)
- [`Email`](#Email)
- [`EmailGroupData`](#EmailGroupData)
- [`EmailQuery`](#EmailQuery)
- [`FieldAccountMetrics`](#FieldAccountMetrics)
- [`FieldAccountMetricsSummary`](#FieldAccountMetricsSummary)
- [`FieldConversions`](#FieldConversions)
- [`FieldGranularConversions`](#FieldGranularConversions)
- [`FieldMetrics`](#FieldMetrics)
- [`FieldMetricsForAdvertisable`](#FieldMetricsForAdvertisable)
- [`FieldMetricsForCampaign`](#FieldMetricsForCampaign)
- [`FieldMetricsTotal`](#FieldMetricsTotal)
- [`FieldUtmBasedConversionsForAdvertisable`](#FieldUtmBasedConversionsForAdvertisable)
- [`FieldsAd`](#FieldsAd)
- [`FieldsAdMetrics`](#FieldsAdMetrics)
- [`FieldsAdgroup`](#FieldsAdgroup)
- [`FieldsAdvertisable`](#FieldsAdvertisable)
- [`FieldsAudience`](#FieldsAudience)
- [`FieldsAudienceMetrics`](#FieldsAudienceMetrics)
- [`FieldsBrandAwarenessForAdvertisables`](#FieldsBrandAwarenessForAdvertisables)
- [`FieldsBrandAwarenessForCampaigns`](#FieldsBrandAwarenessForCampaigns)
- [`FieldsCTVHouseholdMetrics`](#FieldsCTVHouseholdMetrics)
- [`FieldsCampaign`](#FieldsCampaign)
- [`FieldsCustomMetrics`](#FieldsCustomMetrics)
- [`FieldsEmail`](#FieldsEmail)
- [`FieldsEmailMetrics`](#FieldsEmailMetrics)
- [`FieldsForUtmBasedConversions`](#FieldsForUtmBasedConversions)
- [`FieldsInfluencedAttributionMetrics`](#FieldsInfluencedAttributionMetrics)
- [`FieldsOrganization`](#FieldsOrganization)
- [`FieldsProspectingMetrics`](#FieldsProspectingMetrics)
- [`FieldsReachFrequencyMetrics`](#FieldsReachFrequencyMetrics)
- [`FieldsReachMetrics`](#FieldsReachMetrics)
- [`FieldsSMSMetrics`](#FieldsSMSMetrics)
- [`FieldsSegment`](#FieldsSegment)
- [`FieldsVideoMetrics`](#FieldsVideoMetrics)
- [`GranularConversion`](#GranularConversion)
- [`GroupListRow`](#GroupListRow)
- [`GroupQuery`](#GroupQuery)
- [`GroupResult`](#GroupResult)
- [`InventoryCampaign`](#InventoryCampaign)
- [`Keyword`](#Keyword)
- [`KeywordResult`](#KeywordResult)
- [`LogEvent`](#LogEvent)
- [`LogItem`](#LogItem)
- [`LogItemData`](#LogItemData)
- [`LogRoot`](#LogRoot)
- [`Metric`](#Metric)
- [`MetricAggregateResult`](#MetricAggregateResult)
- [`MetricCountry`](#MetricCountry)
- [`MetricCountryResult`](#MetricCountryResult)
- [`MetricDomain`](#MetricDomain)
- [`MetricDomainResult`](#MetricDomainResult)
- [`MetricForAdvertisable`](#MetricForAdvertisable)
- [`MetricForCampaign`](#MetricForCampaign)
- [`MetricResult`](#MetricResult)
- [`Organization`](#Organization)
- [`OrganizationGroupData`](#OrganizationGroupData)
- [`OrganizationQuery`](#OrganizationQuery)
- [`PerformanceTarget`](#PerformanceTarget)
- [`Placement`](#Placement)
- [`PlacementResult`](#PlacementResult)
- [`Query`](#Query)
- [`Segment`](#Segment)
- [`SegmentGroupData`](#SegmentGroupData)
- [`SegmentQuery`](#SegmentQuery)
- [`User`](#User)
- [`UtmBasedConversionsForAdvertisable`](#UtmBasedConversionsForAdvertisable)
- [`UtmBasedConversionsForCampaign`](#UtmBasedConversionsForCampaign)

### Descriptions

### Ad

**Fields**:

### eid: !

EID of the ad.

### adFormatID: !

The id of the corresponding ad format in the AdRoll system.

### adFormat: !

Format string. i.e. ‘300 wide x 250 high’.

### adFormatName: !

Format string. i.e. ‘300x250’.

### advertisable: !

The EID of the advertisable to which this ad belongs.

### hasFutureCampaigns: !

Whether or not this ad has the possibility of serving based on the adgroups and campaigns in which it inhabits.

DEPRECATED: this field will stop being supported in the near future.

### destinationURL: !

The URL that the browser will navigate to when this ad is clicked.

### headline: !

For Facebook ads, the text to be displayed as the ad’s headline.

### body: !

For Facebook ads, the text to be displayed as the ad’s body.

### message: !

For Facebook Newsfeed ads, the text to be displayed as the ad’s message.

### callToAction: !

Facebook call to action constant.

### isActive: !

Whether or not this ad is currently active.

### name: !

The name of this ad.

### src: !

This ad’s creative’s source URL.

### previewURL: !

The preview URL for dynamic ads like HTML5.

### status: !

One of ‘running’, ‘paused’, ‘review’, ‘draft’, ‘rejected’, ‘suspended’ or ‘deleted’.

### actualStatus:

The effective status of the campaign.
Details the reasons why it is not running, if applicable.

### actualStatusString: !

Minimal string representation of the actual status. One of ‘running’,
‘notRunning’ ,’ended’, ‘paused’, ‘review’, ‘draft’, ‘rejected’ or ‘deleted’.

### type: !

The ad type: ‘liquid’, ‘image’, ‘flash’ or ‘ad_network’.

### height: !

The height in pixels of this ad’s creative.

### width: !

The width in pixels of this ad’s creative.

### createdDate:

The date this ad was created.

### updatedDate:

The date this ad was last updated.

### hasEdits: !

Whether or not this ad has been edited such that another ad has it’s original ad parameter set to this ad’s EID.

### hasPendingEdits: !

Whether or not this ad has edits that must be reviewed by an AdRoll administrator.

### originalAd: !

The EID of the ad that was edited to create this ad.

### isDynamic: !

Whether or not this is an ad that is dynamically composed when it is served to the user.

### isOutlined: !

Whether or not an outline has been applied to the ad to satisfy network compliancy.

### outlineColor: !

Hexadecimal color code corresponding to the outline of an ad.

### validClicktag: !

If the ad is in flash format, this is the flag showing whether or not the clickTAG is compliant.

### facebookAdsManagerPermalink: !

DEPRECATED: please use adsManagerPermalink instead

### adsManagerPermalink: !

The URL to the ad if it has been externally connected.

### facebookPermalink: !

Facebook permalink if applicable.

### instagramPermalink: !

Instagram permalink if applicable.

### linkedInPermalink: !

LinkedIn permalink if applicable.

### syncStatus: !

Only for Connected Campaigns’ ads, indicates the status of the sync’ing with the external service.
When available, can be one of “pending”, “synced” or “error”

### syncError: !

Only for Connected Campaigns’ ads, shows the error that caused the sync’ing with the external service to fail.
Provided if the syncStatus field is “error”.

### remoteStatus: !

The status of the Ad on the inventory network NextRoll has sync’ed it to (ex: Facebook)

### disapprovalReason: !

The reason why an Ad has been rejected on the inventory network NextRoll has sync’ed it to (ex: Facebook)

### utmSource: !

UTM Source Parameter from this Ad’s destination.

### utmMedium: !

UTM Medium Parameter from this Ad’s destination.

### utmCampaign: !

UTM Campaign Parameter from this Ad’s destination.

### utmTerm: !

UTM Term Parameter from this Ad’s destination.

### utmContent: !

UTM Content Parameter from this Ad’s destination.

### channel: !

The channel for the campaign this ad belongs to. This is only
available when loading the ads through a campaign.

### campaignType: !

The type for the campaign this ad belongs to. This is only
available when loading the ads through a campaign.

### adrollEID: !

The adroll EID for prospecting ads.

### adcrabEID: !

The AdCrab ad EID for this ad (ending in 8ADS).

### inAdgroupEID: !

The AdGroup’s EID in the AdGroupAd relationship, if listed
inside an AdGroup.

### inAdgroupIsActive: !

True of the AdGroupAd relationship is active, if listed inside
an AdGroup.

### inAdgroupStatus: !

The status of the AdGroupAd relationship, if listed inside
an AdGroup.

### inAdgroupRelationshipEID: !

The the internal EID of the AdGroupAd relationship, if such a EID
exists and if the ad is listed inside an AdGroup.

### labels: []!

The list of custom labels to organize and filter the ad.

### labelsString: !

The list of custom labels as String. e.g.: “label1, label2”

### metrics(start: , end: , pastDays: , currency: , duration:) : !

Metrics for the entity.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The
date range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The
date range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### duration:

[DEPRECATED] Unused.

* **Default:**
  30

### conversions(start: , end: , pastDays: , currency:) : !

Metrics for the entity broken down by conversion audiences.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The date
range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The date
range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### metricsTotal:

Provides aggregation for any metrics in the current and child
nodes.

Note that this will not load the metrics by itself, instead it
aggregates loaded metrics fields in its scope.

For details see the documentation of MetricAggregateResult.

### AdGroupData

**Fields**:

### eid: !

EID of the ad.

### adFormatID: !

The id of the corresponding ad format in the AdRoll system.

### adFormat: !

Format string. i.e. ‘300 wide x 250 high’.

### adFormatName: !

Format string. i.e. ‘300x250’.

### advertisable: !

The EID of the advertisable to which this ad belongs.

### hasFutureCampaigns: !

Whether or not this ad has the possibility of serving based on the adgroups and campaigns in which it inhabits.

DEPRECATED: this field will stop being supported in the near future.

### destinationURL: !

The URL that the browser will navigate to when this ad is clicked.

### headline: !

For Facebook ads, the text to be displayed as the ad’s headline.

### body: !

For Facebook ads, the text to be displayed as the ad’s body.

### message: !

For Facebook Newsfeed ads, the text to be displayed as the ad’s message.

### callToAction: !

Facebook call to action constant.

### isActive: !

Whether or not this ad is currently active.

### name: !

The name of this ad.

### src: !

This ad’s creative’s source URL.

### previewURL: !

The preview URL for dynamic ads like HTML5.

### status: !

One of ‘running’, ‘paused’, ‘review’, ‘draft’, ‘rejected’, ‘suspended’ or ‘deleted’.

### actualStatus:

The effective status of the campaign.
Details the reasons why it is not running, if applicable.

### actualStatusString: !

Minimal string representation of the actual status. One of ‘running’,
‘notRunning’ ,’ended’, ‘paused’, ‘review’, ‘draft’, ‘rejected’ or ‘deleted’.

### type: !

The ad type: ‘liquid’, ‘image’, ‘flash’ or ‘ad_network’.

### height: !

The height in pixels of this ad’s creative.

### width: !

The width in pixels of this ad’s creative.

### createdDate:

The date this ad was created.

### updatedDate:

The date this ad was last updated.

### hasEdits: !

Whether or not this ad has been edited such that another ad has it’s original ad parameter set to this ad’s EID.

### hasPendingEdits: !

Whether or not this ad has edits that must be reviewed by an AdRoll administrator.

### originalAd: !

The EID of the ad that was edited to create this ad.

### isDynamic: !

Whether or not this is an ad that is dynamically composed when it is served to the user.

### isOutlined: !

Whether or not an outline has been applied to the ad to satisfy network compliancy.

### outlineColor: !

Hexadecimal color code corresponding to the outline of an ad.

### validClicktag: !

If the ad is in flash format, this is the flag showing whether or not the clickTAG is compliant.

### facebookAdsManagerPermalink: !

DEPRECATED: please use adsManagerPermalink instead

### adsManagerPermalink: !

The URL to the ad if it has been externally connected.

### facebookPermalink: !

Facebook permalink if applicable.

### instagramPermalink: !

Instagram permalink if applicable.

### linkedInPermalink: !

LinkedIn permalink if applicable.

### syncStatus: !

Only for Connected Campaigns’ ads, indicates the status of the sync’ing with the external service.
When available, can be one of “pending”, “synced” or “error”

### syncError: !

Only for Connected Campaigns’ ads, shows the error that caused the sync’ing with the external service to fail.
Provided if the syncStatus field is “error”.

### remoteStatus: !

The status of the Ad on the inventory network NextRoll has sync’ed it to (ex: Facebook)

### disapprovalReason: !

The reason why an Ad has been rejected on the inventory network NextRoll has sync’ed it to (ex: Facebook)

### utmSource: !

UTM Source Parameter from this Ad’s destination.

### utmMedium: !

UTM Medium Parameter from this Ad’s destination.

### utmCampaign: !

UTM Campaign Parameter from this Ad’s destination.

### utmTerm: !

UTM Term Parameter from this Ad’s destination.

### utmContent: !

UTM Content Parameter from this Ad’s destination.

### channel: !

The channel for the campaign this ad belongs to. This is only
available when loading the ads through a campaign.

### campaignType: !

The type for the campaign this ad belongs to. This is only
available when loading the ads through a campaign.

### adrollEID: !

The adroll EID for prospecting ads.

### adcrabEID: !

The AdCrab ad EID for this ad (ending in 8ADS).

### inAdgroupEID: !

The AdGroup’s EID in the AdGroupAd relationship, if listed
inside an AdGroup.

### inAdgroupIsActive: !

True of the AdGroupAd relationship is active, if listed inside
an AdGroup.

### inAdgroupStatus: !

The status of the AdGroupAd relationship, if listed inside
an AdGroup.

### inAdgroupRelationshipEID: !

The the internal EID of the AdGroupAd relationship, if such a EID
exists and if the ad is listed inside an AdGroup.

### labels: []!

The list of custom labels to organize and filter the ad.

### labelsString: !

The list of custom labels as String. e.g.: “label1, label2”

### AdLabel

**Fields**:

### eid: !

Label EID.

### name: !

Label name.

### AdQuery

**Fields**:

### byEID(ad: !):

Resolves an Ad by its EID.

[WARNING] Fetching Ads directly through this operation will ignore
the overrides and state provided by its relationship to an AdGroup.
For a complete state fetch ads as children of Adgroups.

**Arguments**:

### ad: !

EID of the Ad.

### byEIDs(eids: [!]!): []!

Resolves Ads by their EIDs.

[WARNING] Fetching Ads directly through this operation will ignore
the overrides and state provided by its relationship to an AdGroup.
For a complete state fetch ads as children of Adgroups.

**Arguments**:

### eids: [!]!

List of Ad EIDs.

### byAdvertisable(advertisable: !, isActive: , statuses: [!], types: [!], width: , height: , createdDateAfterOrOn: , createdDateBefore: , updatedDateAfterOrOn: , updatedDateBefore:) : []!

Resolves all Ads for an Advertisable.

[WARNING] Fetching Ads directly through this operation will ignore
the overrides and state provided by its relationship to an AdGroup.
For a complete state fetch ads as children of Adgroups.

**Arguments**:

### advertisable: !

The EID of the advertisable whose ads are to be fetched

### isActive:

If True, only active ads will be returned, and vice versa (Optional; default: True)

### statuses: [!]

Only ads that match one of these statuses will be returned (Optional; default: None)

* **Default:**
  [ ]

### types: [!]

Only ads that match one of these types will be returned (Optional; default: None)

* **Default:**
  [ ]

### width:

Only ads having the specified width will be returned (Optional; default: None)

* **Default:**
  0

### height:

Only ads having the specified height will be returned (Optional; default: None)

* **Default:**
  0

### createdDateAfterOrOn:

Only ads that were created after on on the given date.
String in ISO Date + Time format.
(Optional; default: None)

* **Default:**
  “”

### createdDateBefore:

Only ads that were created before on on the given date.
It will do a less than or equal to string comparison. Reminder that startDate is a ISO timestamp.
(Optional; default: None)

* **Default:**
  “”

### updatedDateAfterOrOn:

Only ads that were updated after on on the given date.
String in ISO Date + Time format.
(Optional; default: None)

* **Default:**
  “”

### updatedDateBefore:

Only ads that were updated before on on the given date.
It will do a less than or equal to string comparison. Reminder that updatedDate is a ISO timestamp.
(Optional; default: None)

* **Default:**
  “”

### byAdgroup(adgroup: !, isActive: , statuses: [!], types: [!], width: , height: , createdDateAfterOrOn: , createdDateBefore: , updatedDateAfterOrOn: , updatedDateBefore:) : []!

Resolves all Ads for an AdGroup.

**Arguments**:

### adgroup: !

The EID of the Adgroup whose ads are to be fetched

### isActive:

If True, only active ads will be returned, and vice versa (Optional; default: True)

### statuses: [!]

Only ads that match one of these statuses will be returned (Optional; default: None)

* **Default:**
  [ ]

### types: [!]

Only ads that match one of these types will be returned (Optional; default: None)

* **Default:**
  [ ]

### width:

Only ads having the specified width will be returned (Optional; default: None)

* **Default:**
  0

### height:

Only ads having the specified height will be returned (Optional; default: None)

* **Default:**
  0

### createdDateAfterOrOn:

Only ads that were created after on on the given date string.
It will do a greater than or equal to string comparison. Reminder that startDate is a ISO timestamp.
(Optional; default: None)

* **Default:**
  “”

### createdDateBefore:

Only ads that were created before on on the given date string.
It will do a less than or equal to string comparison. Reminder that startDate is a ISO timestamp.
(Optional; default: None)

* **Default:**
  “”

### updatedDateAfterOrOn:

Only ads that were updated after on on the given date.
String in ISO Date + Time format.
(Optional; default: None)

* **Default:**
  “”

### updatedDateBefore:

Only ads that were updated before on on the given date.
It will do a less than or equal to string comparison. Reminder that updatedDate is a ISO timestamp.
(Optional; default: None)

* **Default:**
  “”

### metricsTotal:

Provides aggregation for any metrics in the current and child
nodes.

Note that this will not load the metrics by itself, instead it
aggregates loaded metrics fields in its scope.

For details see the documentation of MetricAggregateResult.

### Adgroup

**Fields**:

### eid: !

The EID of the adgroup.

### adOptimization: !

The strategy used to optimize ads when multiple ads fit a single ad space.

### campaign: !

The EID of the campaign that this adgroup is associated with.

### isActive: !

Whether or not this adgroup is currently active.

### name: !

The name of this adgroup.

### status: !

One of ‘approved’, ‘paused’, ‘draft’, ‘rejected’ or ‘deleted’.

### actualStatus:

The effective status of the adgroup.
Details the reasons why it is not running, if applicable.

### actualStatusString: !

Minimal string representation of the actual status. One of
‘running’, ‘notRunning’ ,’ended’, ‘paused’, ‘review’, ‘draft’,
‘rejected’ or ‘deleted’.

### createdDate:

The date this adgroup was created.

### updatedDate:

The date this adgroup was last updated.

### flightTimezone: !

The timezone preference of all flights of this adgroup.

### flights:

Scheduled flight periods when ads will be served. Null if there is no limitation.

### processingStatus: !

The processing status of the campaign inside the AdRoll.
It may have a transient value other than “created” while
the AdGroup is being processed by an internal job.

### significantFlightStartDate:

Start date for the active or most recent flight period in the adgroup.

### significantFlightEndDate:

End date for the active or most recent flight period in the adgroup.

### advertisable: !

Advertisable for this Adgroup. NOTE/FIXME: the advertisable
information is not usually available, so querying this will
cause an additional request to be made.

### kpiGoal:

Goal -for the kpiMetric- that drives the campaign’s bid strategy.
Null for automatic.

### kpiCurrency: !

ISO 4217 currency code for kpiGoal.
If not provided assume the currency provided at the Advertisable level.

### kpiMetric: !

Metric being targeted by the campaign’s bid strategy.

### adType: !

Ad type restriction for this adgroup.
Empty if there is no explicit restriction. Currently one of “static”or “dynamic.

### facebookAdsManagerPermalink: !

DEPRECATED: please use adsManagerPermalink instead

### adsManagerPermalink: !

The URL to the adgroup if it has been externally connected.

### syncStatus: !

Only for Connected Campaigns’ adgroups, indicates the status of the sync’ing with the external service.
When available, can be one of “pending”, “synced” or “error”

### syncError: !

Only for Connected Campaigns’ adgroups, shows the error that caused the sync’ing with the external service to fail.
Provided if the syncStatus field is “error”.

### allowedTargeting: !

The allowed targeting type configured for this adgroup.

### ads(isActive: , statuses: [!], types: [!], width: , height: , createdDateAfterOrOn: , createdDateBefore: , updatedDateAfterOrOn: , updatedDateBefore:) : []!

Ads for this Adgroup.

**Arguments**:

### isActive:

If True, only active ads will be returned, and vice versa (Optional; default: True)

### statuses: [!]

Only ads that match one of these statuses will be returned (Optional; default: None)

* **Default:**
  [ ]

### types: [!]

Only ads that match one of these types will be returned (Optional; default: None)

* **Default:**
  [ ]

### width:

Only ads having the specified width will be returned (Optional; default: None)

* **Default:**
  0

### height:

Only ads having the specified height will be returned (Optional; default: None)

* **Default:**
  0

### createdDateAfterOrOn:

Only ads that were created after on on the given date string.
It will do a greater than or equal to string comparison. Reminder that startDate is a ISO timestamp.
(Optional; default: None)

* **Default:**
  “”

### createdDateBefore:

Only ads that were created before on on the given date string.
It will do a less than or equal to string comparison. Reminder that startDate is a ISO timestamp.
(Optional; default: None)

* **Default:**
  “”

### updatedDateAfterOrOn:

Only ads that were updated after on on the given date.
String in ISO Date + Time format.
(Optional; default: None)

* **Default:**
  “”

### updatedDateBefore:

Only ads that were updated before on on the given date.
It will do a less than or equal to string comparison. Reminder that updatedDate is a ISO timestamp.
(Optional; default: None)

* **Default:**
  “”

### audiences(includeInactive:) : []!

Audiences for this Adgroup

**Arguments**:

### includeInactive:

True to return also inactive audiences (those that have been deleted).
By default only active audiences are included.

* **Default:**
  false

### metrics(start: , end: , pastDays: , currency: , duration:) : !

Metrics for the entity.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The
date range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The
date range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### duration:

[DEPRECATED] Unused.

* **Default:**
  30

### placements(start: , end: , pastDays: , currency:) : !

Metrics for the AdGroup broken down by conversion audiences.
This breakdown will only be provided for Facebook campaigns.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The date
range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The date
range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### ctvPlacements(start: , end: , pastDays: , breakdown: !, currency:) : !

CTV Metrics for the AdGroup.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The date
range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The date
range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### breakdown: !

The breakdown value used for ctv placement metrics. One of [‘app_name’, ‘publisher’, ‘device_make’].

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### contextualTargeting(start: , end: , pastDays: , currency:) : !

[ALPHA] This GraphQL field is currently under development and QA
Contextual Targeting Metrics for the AdGroup.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The date
range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The date
range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### keywords(start: , end: , pastDays: , currency:) : !

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Currently Fetching Keywords and keyword metrics without also
requesting metrics for parent adgroup or campaign will return empty result.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The date
range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The date
range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### conversions(start: , end: , pastDays: , currency:) : !

Metrics for the entity broken down by conversion audiences.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The date
range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The date
range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### metricsTotal:

Provides aggregation for any metrics in the current and child
nodes.

Note that this will not load the metrics by itself, instead it
aggregates loaded metrics fields in its scope.

For details see the documentation of MetricAggregateResult.

### AdgroupGroupData

**Fields**:

### eid: !

The EID of the adgroup.

### adOptimization: !

The strategy used to optimize ads when multiple ads fit a single ad space.

### campaign: !

The EID of the campaign that this adgroup is associated with.

### isActive: !

Whether or not this adgroup is currently active.

### name: !

The name of this adgroup.

### status: !

One of ‘approved’, ‘paused’, ‘draft’, ‘rejected’ or ‘deleted’.

### actualStatus:

The effective status of the adgroup.
Details the reasons why it is not running, if applicable.

### actualStatusString: !

Minimal string representation of the actual status. One of
‘running’, ‘notRunning’ ,’ended’, ‘paused’, ‘review’, ‘draft’,
‘rejected’ or ‘deleted’.

### createdDate:

The date this adgroup was created.

### updatedDate:

The date this adgroup was last updated.

### flightTimezone: !

The timezone preference of all flights of this adgroup.

### flights:

Scheduled flight periods when ads will be served. Null if there is no limitation.

### processingStatus: !

The processing status of the campaign inside the AdRoll.
It may have a transient value other than “created” while
the AdGroup is being processed by an internal job.

### significantFlightStartDate:

Start date for the active or most recent flight period in the adgroup.

### significantFlightEndDate:

End date for the active or most recent flight period in the adgroup.

### advertisable: !

Advertisable for this Adgroup. NOTE/FIXME: the advertisable
information is not usually available, so querying this will
cause an additional request to be made.

### kpiGoal:

Goal -for the kpiMetric- that drives the campaign’s bid strategy.
Null for automatic.

### kpiCurrency: !

ISO 4217 currency code for kpiGoal.
If not provided assume the currency provided at the Advertisable level.

### kpiMetric: !

Metric being targeted by the campaign’s bid strategy.

### adType: !

Ad type restriction for this adgroup.
Empty if there is no explicit restriction. Currently one of “static”or “dynamic.

### facebookAdsManagerPermalink: !

DEPRECATED: please use adsManagerPermalink instead

### adsManagerPermalink: !

The URL to the adgroup if it has been externally connected.

### syncStatus: !

Only for Connected Campaigns’ adgroups, indicates the status of the sync’ing with the external service.
When available, can be one of “pending”, “synced” or “error”

### syncError: !

Only for Connected Campaigns’ adgroups, shows the error that caused the sync’ing with the external service to fail.
Provided if the syncStatus field is “error”.

### allowedTargeting: !

The allowed targeting type configured for this adgroup.

### AdgroupQuery

**Fields**:

### byEID(adgroup: !):

Resolves an Adgroup by its EID.

**Arguments**:

### adgroup: !

EID of the Adgroup.

### byEIDs(eids: [!]!): []!

Resolves a Adgroups by their EIDs.

**Arguments**:

### eids: [!]!

List of Campaign EIDs.

### byAdvertisable(advertisable: !, isActive: , statuses: [!], excludeStatuses: [!]): []!

Resolves all Adgroups for a Advertisable.

**Arguments**:

### advertisable: !

The EID of the advertisable whose adgroups are to be fetched

### isActive:

If True, only active adgroups will be returned, and vice versa (Optional; default: True)

### statuses: [!]

Only adgroups that match one of these statuses will be returned (Optional; default: None)

* **Default:**
  [ ]

### excludeStatuses: [!]

Only adgroups whose status is not one of these will be returned (Optional; default: None)

* **Default:**
  [ ]

### byCampaign(campaign: !, isActive: , statuses: [!], excludeStatuses: [!]): []!

Resolves all Adgroups for a Campaign.

**Arguments**:

### campaign: !

EID of the campaign.

### isActive:

If True, only active adgroups will be returned, and vice versa (Optional; default: True)

### statuses: [!]

Only adgroups that match one of these statuses will be returned (Optional; default: None)

* **Default:**
  [ ]

### excludeStatuses: [!]

Only adgroups whose status is not one of these will be returned (Optional; default: None)

* **Default:**
  [ ]

### metricsTotal:

Provides aggregation for any metrics in the current and child
nodes.

Note that this will not load the metrics by itself, instead it
aggregates loaded metrics fields in its scope.

For details see the documentation of MetricAggregateResult.

### Advertisable

**Fields**:

### eid: !

EID of the advertisable.

### isActive: !

Whether or not the advertisable is currently active.

### isB2B: !

Whether or not the advertisable is a B2B customer.
Deprecated field: use businessUnit instead.

### businessUnit: !

The business unit this Advertisable has signed up for.

### isAbmCustomer: !

Whether or not the advertisable is an ABM customer.

### name: !

The name of the advertisable.

### organization: !

The EID of this advertisable’s organization.

### status: !

The status of the advertisable. One of [‘admin_review’, ‘approved’, ‘rejected’, ‘suspended’].

### url: !

The advertisable’s URL.

### currency: !

The currency code (ISO-4217) use by the advertisable’s account.

### clickThroughConversionWindow: !

Duration of this advertisable’s click through conversion window in days.

### viewThroughConversionWindow: !

Duration of this advertisable’s view through conversion window in days.

### createdDate:

The date this advertisable was created.

### revshareViewPercent: !

### revshareClickPercent: !

### campaigns(isActive: , statuses: [!], excludeStatuses: [!], blacklistStatuses: [!], useCases: [!], types: [!], targetingTypes: [!], abmTypes: [!], channels: [!], sources: [!], funnelStages: [!], objectives: [!], excludeUseCases: [!], excludeTypes: [!], excludeTargetingTypes: [!], excludeABMTypes: [!], excludeChannels: [!], excludeSources: [!], excludeFunnelStages: [!], tagPrefixes: [!]): []!

Campaigns for this Advertisable.

**Arguments**:

### isActive:

If True, only active campaigns will be returned, and vice versa (Optional; default: True)

### statuses: [!]

Only campaigns that match one of these statuses will be returned (Optional; default: None)

* **Default:**
  [ ]

### excludeStatuses: [!]

Only campaigns whose status is not one of these will be returned (Optional; default: None)

* **Default:**
  [ ]

### blacklistStatuses: [!]

DEPRECATED: please use instead argument excludeStatuses

* **Default:**
  [ ]

### useCases: [!]

Only campaigns that match one of these use cases will be returned (Optional; default: None)

* **Default:**
  [ ]

### types: [!]

Only campaigns that match one of these types will be returned (Optional; default: None)

* **Default:**
  [ ]

### targetingTypes: [!]

Only campaigns that match one of these targeting types will be returned (Optional; default: None)

* **Default:**
  [ ]

### abmTypes: [!]

Only campaigns that match one of these ABM types will be returned. Options: ‘lead_locator’ for Account Targeting, ‘pipeline_accelerator’ for Contact-based. (Optional; default: None)

* **Default:**
  [ ]

### channels: [!]

Only campaigns that match one of these channels will be returned (Optional; default: None)

* **Default:**
  [ ]

### sources: [!]

Only campaigns that match one of these sources will be returned (Optional; default: None)

* **Default:**
  [ ]

### funnelStages: [!]

Only campaigns that match one of these funnel stages will be returned (Optional; default: None)

* **Default:**
  [ ]

### objectives: [!]

Only campaigns that match one of these objectives will be returned (Optional; default: None)

* **Default:**
  [ ]

### excludeUseCases: [!]

Exclude campaigns that match one of the given use cases (Optional; default: None)

* **Default:**
  [ ]

### excludeTypes: [!]

Exclude campaigns that match one of the given types. (Optional; default: None)

* **Default:**
  [ ]

### excludeTargetingTypes: [!]

Exclude campaigns that match one of the given targeting types. (Optional; default: None)

* **Default:**
  [ ]

### excludeABMTypes: [!]

Exclude campaigns that match one of the given ABM types. (Optional; default: None)

* **Default:**
  [ ]

### excludeChannels: [!]

Exclude campaigns that match one of the given channels. (Optional; default: None)

* **Default:**
  [ ]

### excludeSources: [!]

Exclude campaigns that match one of the given sources. (Optional; default: None)

* **Default:**
  [ ]

### excludeFunnelStages: [!]

Exclude campaigns that match one of the given funnel stages. (Optional; default: None)

* **Default:**
  [ ]

### tagPrefixes: [!]

> Only campaigns that have tags that start with one of the given prefixes. (Optional; default: None)
* **Default:**
  [ ]

### automations: []!

Automations for this Advertisable.

### adgroups(isActive: , statuses: [!], excludeStatuses: [!]): []!

Adgroups for this Advertisable.

**Arguments**:

### isActive:

If True, only active adgroups will be returned, and vice versa (Optional; default: True)

### statuses: [!]

Only adgroups that match one of these statuses will be returned (Optional; default: None)

* **Default:**
  [ ]

### excludeStatuses: [!]

Only adgroups whose status is not one of these will be returned (Optional; default: None)

* **Default:**
  [ ]

### emails: []!

Emails for this Advertisable.

### ads(isActive: , statuses: [!], types: [!], width: , height: , createdDateAfterOrOn: , createdDateBefore: , updatedDateAfterOrOn: , updatedDateBefore:) : []!

Ads for this Advertisable.

**Arguments**:

### isActive:

If True, only active ads will be returned, and vice versa (Optional; default: False)

### statuses: [!]

Only ads that match one of these statuses will be returned (Optional; default: None)

* **Default:**
  [ ]

### types: [!]

Only ads that match one of these types will be returned (Optional; default: None)

* **Default:**
  [ ]

### width:

Only ads having the specified width will be returned (Optional; default: None)

* **Default:**
  0

### height:

Only ads having the specified height will be returned (Optional; default: None)

* **Default:**
  0

### createdDateAfterOrOn:

Only ads that were created after on on the given date string.
It will do a greater than or equal to string comparison. Reminder that startDate is a ISO timestamp.
(Optional; default: None)

* **Default:**
  “”

### createdDateBefore:

Only ads that were created before on on the given date string.
It will do a less than or equal to string comparison. Reminder that startDate is a ISO timestamp.
(Optional; default: None)

* **Default:**
  “”

### updatedDateAfterOrOn:

Only ads that were updated after on on the given date.
String in ISO Date + Time format.
(Optional; default: None)

* **Default:**
  “”

### updatedDateBefore:

Only ads that were updated before on on the given date.
It will do a less than or equal to string comparison. Reminder that updatedDate is a ISO timestamp.
(Optional; default: None)

* **Default:**
  “”

### segments(isActive: , isConversion:) : []!

Segments for this Advertisable.

**Arguments**:

### isActive:

If True, only active segments will be returned, and vice versa (Optional; default: False)

### isConversion:

If True, only conversion segments will be returned (Optional; default: False).

### metrics(start: , end: , pastDays: , currency: , duration:) : !

Metrics for the Advertisable.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The
date range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The
date range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### duration:

[DEPRECATED] Unused.

* **Default:**
  30

### conversions(start: , end: , pastDays: , currency:) : !

Metrics for the entity broken down by conversion audiences.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The date
range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The date
range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### metricsTotal:

Provides aggregation for any metrics in the current and child
nodes.

Note that this will not load the metrics by itself, instead it
aggregates loaded metrics fields in its scope.

For details see the documentation of MetricAggregateResult.

### granularConversions(start: , end: , pastDays: , currency:) : [!]!

The granular conversions help understand the channels, campaigns, and ads that influence conversions.
Lists the details about a conversion and the data points that determined the decision about its attribution.
Limited to 90 days.

**Arguments**:

### start:

The start date for the conversions period (inclusive).
The date range will be: [start, end)

### end:

The end date for the conversions period (exclusive).
The date range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the conversions in.

* **Default:**
  “USD”

### utmBasedConversions(start: , end: , pastDays: , currency: , model: !): [!]!

UTM based conversions for the Advertisable.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The
date range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The
date range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### model: !

Model can be one of the following:
[utm_firsttouch, utm_lastclick, utm_lasttouch, utm_linear, utm_positional, utm_timedecay]

### AdvertisableGroupData

**Fields**:

### eid: !

EID of the advertisable.

### isActive: !

Whether or not the advertisable is currently active.

### isB2B: !

Whether or not the advertisable is a B2B customer.
Deprecated field: use businessUnit instead.

### businessUnit: !

The business unit this Advertisable has signed up for.

### isAbmCustomer: !

Whether or not the advertisable is an ABM customer.

### name: !

The name of the advertisable.

### organization: !

The EID of this advertisable’s organization.

### status: !

The status of the advertisable. One of [‘admin_review’, ‘approved’, ‘rejected’, ‘suspended’].

### url: !

The advertisable’s URL.

### currency: !

The currency code (ISO-4217) use by the advertisable’s account.

### clickThroughConversionWindow: !

Duration of this advertisable’s click through conversion window in days.

### viewThroughConversionWindow: !

Duration of this advertisable’s view through conversion window in days.

### createdDate:

The date this advertisable was created.

### revshareViewPercent: !

### revshareClickPercent: !

### AdvertisableMetricResult

Groups reporting metric data in summary, by date and by domain format.

**Fields**:

### summary: !

Summarizes the reporting data for the given date range.

### byDate: [!]!

Reporting data by date in the given range.

### byDomain: [!]!

Reporting data by domain.

### AdvertisableQuery

**Fields**:

### byEID(advertisable: !):

Obtain an Advertisable by its unique identifier (EID).

**Arguments**:

### advertisable: !

Advertisable EID.

### byEIDs(eids: [!]!): []!

Obtain a list of Advertisables by their unique identifiers (EID).

**Arguments**:

### eids: [!]!

List of Advertisable EIDs.

### byOrganization(organization: !): []!

Obtain a list Advertisables owned by an Organization.

**Arguments**:

### organization: !

Organization EID.

### forUser: []!

All the advertisables for the current user.

### metricsTotal:

Provides aggregation for any metrics in the current and child
nodes.

Note that this will not load the metrics by itself, instead it
aggregates loaded metrics fields in its scope.

For details see the documentation of MetricAggregateResult.

### Audience

**Fields**:

### eid: !

The EID of the audience in use.

### segmentEID: !

The EID of the segment describing this audience.

### advertisable: !

The Advertisable for the segment.

### campaign: !

The Campaign for the segment.

### name: !

The Audience Name.

### type: !

The type of the segment. One of:
- “url”: URL
- “crm”: crm
- “pages_viewed”: Pages Viewed
- “products_viewed”: Products Viewed
- “arbitrary_data”: External Data
- “app_install”: App Install
- “facebook_prospecting”: Facebook Prospecting
- “custom”: Partner
- “intent”: Intent
- “impression”: Impression
- “user_attributes”: Attributes
- “user_events”: Events
- “lead_generation”: Lead Generation
- “composite”: Composite
- “event_match”: Event JS Match
- “js_match”: Explicit JS Match
- “ipixel_match”: IPixel Match
- “css_selector”: CSS Selector
- “email_list”: Email List in AdRoll Email.
- “email_domain”: Email Address Domain Match.

### tags: !

Tags explicitly assigned to the segment.

### description: !

Pieces to build the Audience’s description formatted following the type.

### duration: !

The duration of the Audience, in days.

### isActive: !

False if this is segment has been deleted.

### inclusion: !

Is the segment an inclusion segment.

### isConversion: !

True if this is a conversion audience.

### conversionValue: !

The value of a conversion from this segment.

### currency: !

The value of a conversion from this segment. Default to the Advertisable’s currency.

### createdDate:

Date of creation.

### product:

Product the segment belongs to.

### metrics(start: , end: , pastDays:) : !

Metrics for the audience visitors.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The date
range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The date
range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### AudienceGroupData

**Fields**:

### eid: !

The EID of the audience in use.

### segmentEID: !

The EID of the segment describing this audience.

### advertisable: !

The Advertisable for the segment.

### campaign: !

The Campaign for the segment.

### name: !

The Audience Name.

### type: !

The type of the segment. One of:
- “url”: URL
- “crm”: crm
- “pages_viewed”: Pages Viewed
- “products_viewed”: Products Viewed
- “arbitrary_data”: External Data
- “app_install”: App Install
- “facebook_prospecting”: Facebook Prospecting
- “custom”: Partner
- “intent”: Intent
- “impression”: Impression
- “user_attributes”: Attributes
- “user_events”: Events
- “lead_generation”: Lead Generation
- “composite”: Composite
- “event_match”: Event JS Match
- “js_match”: Explicit JS Match
- “ipixel_match”: IPixel Match
- “css_selector”: CSS Selector
- “email_list”: Email List in AdRoll Email.
- “email_domain”: Email Address Domain Match.

### tags: !

Tags explicitly assigned to the segment.

### description: !

Pieces to build the Audience’s description formatted following the type.

### duration: !

The duration of the Audience, in days.

### isActive: !

False if this is segment has been deleted.

### inclusion: !

Is the segment an inclusion segment.

### isConversion: !

True if this is a conversion audience.

### conversionValue: !

The value of a conversion from this segment.

### currency: !

The value of a conversion from this segment. Default to the Advertisable’s currency.

### createdDate:

Date of creation.

### product:

Product the segment belongs to.

### AudienceMetric

Groups reporting metric audience data in summary and by date format.

**Fields**:

### audienceSizeCurrent: !

Total number of unique visitors within the duration of the segment.
i.e. [TODAY - DURATION, TODAY).

This is the total number of visitors who can be retargeted using this segment.

### audienceSizeNew: !

[DEPRECATED] Please use the other metrics in this node instead.
Count of unique new visitors who visited the entities between the specified date range.

### audienceSizeTotal: !

Total number of unique visitors between the specified start date (inclusive) and end date (exclusive)
ignoring the segment’s own duration.
i.e. [START_DATE, END_DATE)

### audienceSizeInDateRange: !

Total number of unique visitors within the duration of the entity with the specified date range.
i.e. [$END_DATE - $DURATION, $END_DATE)

### AudienceMetricResult

Groups reporting metric audience data in summary and by date format.

**Fields**:

### summary: !

Summarizes the reporting data for the given date range and duration.

### Automation

**Fields**:

### eid: !

EID of the automation.

### name: !

Name of the automation.

### advertisable: !

EID of the advertisable to which this automation belongs to.

### isActive: !

False if the automation has been marked as deleted.

### createdDate:

The timestamp for when this automation was created.

### updatedDate:

The timestamp for when this automation was last modified.

### firstLaunchDate:

The timestamp for the first time that a node was successfully launched from this automation

### entrySegmentEID: !

EID of the base internal segment that includes contacts in the automation.

### exitSegmentEID: !

EID of the base internal segment that removes contacts in the automation.

### templateEID:

EID of the template originally used to create this automation.

### triggerRules: !

### exclusionRules: !

### classification: !

Classification for the automation. A non-localized constant identifying the automation’s type.

### funnelStage: !

Funnel stage for the automation. One of ‘awareness’, ‘consideration’, ‘conversion’, or ‘other’.

### actualStatus:

Actual status derived from the actual statuses of the child Campaigns

### actualStatusString: !

Minimal string representation of the actual status.

### emailCampaignEID:

EID of the email campaign that backs the emails in this automation.

### emailCampaign:

### smsCampaignEID:

[DEPRECATED] The SMS API backing this field has been retired. This field
always returns null.

### smsCampaign:

[DEPRECATED] The SMS API backing this field has been retired. This field
always returns null.

### entryAudiences:

### exitAudiences:

### nodes: []!

### metrics(start: , end: , pastDays: , currency: , duration:) : !

Metrics for the Campaign.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The
date range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The
date range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### duration:

[DEPRECATED] Unused.

* **Default:**
  30

### conversions(start: , end: , pastDays: , currency:) : !

Metrics for the entity broken down by conversion audiences.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The date
range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The date
range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### metricsTotal:

Provides aggregation for any metrics in the current and child
nodes.

Note that this will not load the metrics by itself, instead it
aggregates loaded metrics fields in its scope.

For details see the documentation of MetricAggregateResult.

### AutomationNode

**Fields**:

### eid: !

EID of the automation node.

### name: !

Name of the automation node.

### advertisable: !

EID of the advertisable to which this automation belongs to.

### automation: !

EID of the automation.

### isRoot: !

True if this node is one of the tree’s roots.

If this is false and parentNodeEID is null, the node is considered detached.

### parentNodeEID:

EID of the parent node that places this node in the tree structure.

### isActive: !

False if the automation has been marked as deleted.

### status: !

Status of the automation node itself, independent from the campaign.

### nodeType: !

One of conditional, campaign_ad, campaign_email, or campaign_sms.

### delayHours: !

Additional time to wait—since the completion of the previous node—before
the contact reaches this node.

### trackOrder: !

Relative order between nodes at the same level.

### createdDate:

The timestamp for when this automation node was created.

### updatedDate:

The timestamp for when this automation node was last modified.

### condition: !

### conditionOperator:

### conditionValue:

### audienceAdditionalRules:

Additional rules to be layered on top of the baseline established by
the Automation’s trigger & exclusion plus the node position on the flow.

### durationHours:

For Ad campaigns, maximum time that the user would be served this campaign.

For delay nodes, the time before the flow can continue.

### entrySegmentEID:

EID of the targeted audience for the node.

### exitSegmentEID:

EID of the excluded audience for the node.

### extensionEntrySegmentEIDs:

Additional segment EIDs that extend the reach of the campaign;’s entry audience

### extensionExitSegmentEIDs:

Additional segment EIDs that extend the reach of the campaign;’s exit audience

### campaignEID:

### campaign:

### emailEID:

### email:

### metrics(start: , end: , pastDays: , currency: , duration:) : !

Metrics for the Campaign.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The
date range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The
date range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### duration:

[DEPRECATED] Unused.

* **Default:**
  30

### conversions(start: , end: , pastDays: , currency:) : !

Metrics for the entity broken down by conversion audiences.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The date
range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The date
range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### metricsTotal:

Provides aggregation for any metrics in the current and child
nodes.

Note that this will not load the metrics by itself, instead it
aggregates loaded metrics fields in its scope.

For details see the documentation of MetricAggregateResult.

### AutomationQuery

**Fields**:

### byEID(automation: !):

**Arguments**:

### automation: !

EID of the automation.

### byEIDs(eids: [!]!): [!]!

**Arguments**:

### eids: [!]!

EIDs of the automations.

### byAdvertisable(advertisable: !, isActive:) : [!]!

**Arguments**:

### advertisable: !

The EID of the advertisable whose campaigns are to be fetched

### isActive:

If True only non-delted automations are included. Default to False

### CTVPlacement

**Fields**:

### placement: !

Placement of the Ad in Connected TV. Depending on the breakdown arg it can be
by App name, seller of device make

### impressions: !

The sum of the number of ad impressions.

### clicks: !

The sum of clicks of ads.

### cost: !

Cost associated to ads.

### cpm: !

Cost per mille.
Cost per one thousand ad serves on the domain.

CPM ($) = Spend / Impressions \* 1000

### videoImpressions:

Impressions from video ads.

### videoViews:

Number of times the video begun playing.

### videoTwentyFivePercent:

Number of times at least 25% of the video duration was played.

### videoFiftyPercent:

Number of times at least 50% of the video duration was played.

### videoSeventyFivePercent:

Number of times at least 75% of the video duration was played.

### videoHundredPercent:

Number of times the full video duration was played.

### videoCompletionRate:

Video completion rate

Video Completion Rate (x) = Video Viewed To 100% / Video Impressions

### CTVPlacementResult

Groups reporting metric data in summary and by date format.

**Fields**:

### byPlacement: [!]!

Summarizes by placement the reporting data for the given date range.

### Campaign

**Fields**:

### eid: !

EID of the campaign.

### advertisable: !

EID of the advertisable to which this campaign belongs.

### budget: !

The daily budget of the campaign.
Note that this can be an approximation, for example when budgetType = “lifetime” it is:
budget = budgetGoal / numberOfDays(budgetStartDate, budgetEndDate)

### budgetGoal: !

The budget of the campaign, considered for the whole extent of its budgetType.
When budgetType = “lifetime”, it will be applied in the period since budgetStartDate until budgetEndDate.

### budgetType: !

The type of budget of the campaign (daily, lifetime…).
If this includes -auto (i.e. daily-auto), then it is the inventory campaign of a proxy strategy that is auto-balancing the budget for this campaign

### budgetStartDate:

The start date of a lifetime budget.

### budgetEndDate:

The end date of a lifetime budget.

### budgetSettingsString: !

Serialized budget settings as a string.
“budgetType,budgetStartDate,budgetEndDate,budgetGoal”

### createdDate:

The date this campaign was created.

### cpc: !

The CPC for this campaign.

### cpm: !

The CPM for this campaign.

### maxCpm: !

The maximum CPM for this campaign.

### name: !

The name of this campaign.

### startDate:

The day the campaign will start.

### endDate:

The day the campaign will end, exclusive.

### status: !

The status of the campaign.
One of ‘running’, ‘ended’, ‘paused’, ‘review’, ‘draft’, ‘rejected’ or ‘deleted’.
Result is ‘billingFailedPermanent’ or ‘billingFailedRecoverable’ when BillingAuthStatus is ‘failed’.

### actualStatus:

The effective status of the campaign.
Details the reasons why it is not running, if applicable.

### actualStatusString: !

Minimal string representation of the actual status.
One of ‘running’, ‘notRunning’ ,’ended’, ‘paused’, ‘review’, ‘draft’, ‘rejected’ or ‘deleted’.

### updatedDate:

The date this campaign was last updated.

### channel: !

Campaign channel: one of ‘email’, ‘social’ or ‘web’

### isConnectedChannel: !

True if the campaign is run by a third party.

### source: !

The service responsible for the creation of this campaign.

### currency: !

ISO-4217 currency code for the given amount.

### type: !

Type for the campaign. One of “prospecting”, “blended”r
“retargeting”.

### abmType: !

Type of ABM campaign.
Empty string if this is not an ABM campaign.

### targetingType: !

The type of targeting that is used to pick which customers will be reached by this campaign.

### kpiGoal: !

Goal -for the kpiMetric- that drives the campaign’s bid strategy.
Null for automatic.

### kpiCurrency: !

ISO 4217 currency code for kpiGoal.
If not provided assume the currency provided at the Advertisable level.

### kpiMetric: !

Metric being targeted by the campaign’s bid strategy.

### spendLimitUntil:

SpendLimitUntil

### spendLimitUntilReason: !

SpendLimitUntilReason

### processingStatus: !

The processing status of the campaign inside the AdRoll.
It may have a transient value other than “created” while
the campaign is being processed by an internal job.

### billingAuthStatus:

The billing auth status of the campaign inside the AdRoll.
Will default to empty string when API BillingAuthStatus not present.
Result is “failed” when the billing authorization did not complete.

### playbookEID: !

The parent Playbook’s EID for the campaign, only if it exists.

### playbookName: !

The parent Playbook’s Name for the campaign, only if it exists.

### playbookType: !

The parent Playbook’s Type for the campaign, only if it exists.

### inVoltronStrategyEID: !

The EID of this campaign as referenced from its Voltron strategy.
Only available for inventory campaigns of Universal Campaigns.

### proxyStrategyEID: !

The eid of the Proxy Strategy that contains this campaign. Only for Inventory campaigns.

### proxyStrategyIsFrozen: !

The isFrozen value of the Proxy Strategy that contains this campaign. Only for Inventory campaigns.

### proxyStrategyStatus: !

The status of the Proxy Strategy that contains this campaign. Only for Inventory campaigns.

### proxyStrategyName: !

The name of the Proxy Strategy that contains this campaign. Only for Inventory campaigns.

### newsletterScheduled: !

If this is an Email Newsletter campaign, the number of potential recipients.

### newsletterSends: !

If this is an Email Newsletter campaign, the number of emails sent.

### newsletterScheduledDate:

If this is an Email Newsletter campaign, the scheduled date for delivery.
Only if the delivery is scheduled to happen or of it has already occurred. Omitted if in draft, paused or cancelled.

### isBillable: !

True if the campaign is run by NextRoll and will be directly billed to
the advertisable’s account. False if it is run by a third party.

### isFrozen: !

True if the strategy is frozen, and no changes can be made to it.

### syncStatus: !

Only for Connected Campaigns, indicates the status of the sync’ing with the external service.
When available, can be one of “pending”, “synced” or “error”

### syncError: !

Only for Connected Campaigns, shows the error that caused the sync’ing with the external service to fail.
Provided if the syncStatus field is “error”.

### facebookAdsManagerPermalink: !

DEPRECATED: please use adsManagerPermalink instead

### adsManagerPermalink: !

The URL to the campaign if it has been externally connected.

### isIntegrated: !

### useCase: !

### objective: !

The campaign marketing objective returned by AdRoll API.

### funnelStage:

Funnel stage for the campaign. One of “awareness”, “consideration”, “conversion”, or “other”.

### isBudgetBalancingAutomated: !

Indicates if this campaign is a strategy that balances the budget automatically across its inventory campaigns.
False means that inventory campaign budgets are manually set.

### possibleStatusChanges: [!]

Available status changes for the current campaign. BETA.

### performanceTargets: []

PerformanceTargets

### tags: [!]

Internal tags set on creation.

### automationEID:

If managed by an Automation, the EID of the Automation.

### automationNodeEID:

If managed by an Automation,
the EID of the Automation Node that references this entity.

### automationName:

If managed by an Automation, the name of the Automation.

### disabled: !

Indicates if the campaign is disabled.
Currently applies only to Automation-managed campaigns that have been disabled by subscription downgrade action.

### klaviyoFlowEID:

If managed by a Klaviyo Flow, the EID of the Flow.

### klaviyoFlowName:

If managed by a Klaviyo Flow, the name of the Flow.

### campaignGroupEID: !

EID for the parent Universal/Proxy campaign group for an inventory campaign.

This is only available if Universal or Proxy campaign are enabled in the query.

### campaignGroupName: !

Name for the parent Universal/Proxy campaign group for an inventory campaign.

This is only available if Universal or Proxy campaign are enabled in the query.

### adgroups(isActive: , statuses: [!], excludeStatuses: [!]): []!

Adgroups for this Campaign.

**Arguments**:

### isActive:

If True, only active adgroups will be returned, and vice versa (Optional; default: True)

### statuses: [!]

Only adgroups that match one of these statuses will be returned (Optional; default: None)

* **Default:**
  [ ]

### excludeStatuses: [!]

Only adgroups whose status is not one of these will be returned (Optional; default: None)

* **Default:**
  [ ]

### emails: []!

Emails for this Campaign

### audiences(includeInactive:) : []!

Audiences for this Campaign.

**Arguments**:

### includeInactive:

True to return also inactive audiences (those that have been deleted).
By default only active audiences are included.

* **Default:**
  false

### metrics(start: , end: , pastDays: , currency: , duration:) : !

Metrics for the Campaign.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The
date range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The
date range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### duration:

[DEPRECATED] Unused.

* **Default:**
  30

### conversions(start: , end: , pastDays: , currency:) : !

Metrics for the entity broken down by conversion audiences.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The date
range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The date
range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### metricsTotal:

Provides aggregation for any metrics in the current and child
nodes.

Note that this will not load the metrics by itself, instead it
aggregates loaded metrics fields in its scope.

For details see the documentation of MetricAggregateResult.

### inventoryCampaigns: []!

Inventory Campaigns that compose this campaign in the case of Proxy Campaigns.

### CampaignGroupData

**Fields**:

### eid: !

EID of the campaign.

### advertisable: !

EID of the advertisable to which this campaign belongs.

### budget: !

The daily budget of the campaign.
Note that this can be an approximation, for example when budgetType = “lifetime” it is:
budget = budgetGoal / numberOfDays(budgetStartDate, budgetEndDate)

### budgetGoal: !

The budget of the campaign, considered for the whole extent of its budgetType.
When budgetType = “lifetime”, it will be applied in the period since budgetStartDate until budgetEndDate.

### budgetType: !

The type of budget of the campaign (daily, lifetime…).
If this includes -auto (i.e. daily-auto), then it is the inventory campaign of a proxy strategy that is auto-balancing the budget for this campaign

### budgetStartDate:

The start date of a lifetime budget.

### budgetEndDate:

The end date of a lifetime budget.

### budgetSettingsString: !

Serialized budget settings as a string.
“budgetType,budgetStartDate,budgetEndDate,budgetGoal”

### createdDate:

The date this campaign was created.

### cpc: !

The CPC for this campaign.

### cpm: !

The CPM for this campaign.

### maxCpm: !

The maximum CPM for this campaign.

### name: !

The name of this campaign.

### startDate:

The day the campaign will start.

### endDate:

The day the campaign will end, exclusive.

### status: !

The status of the campaign.
One of ‘running’, ‘ended’, ‘paused’, ‘review’, ‘draft’, ‘rejected’ or ‘deleted’.
Result is ‘billingFailedPermanent’ or ‘billingFailedRecoverable’ when BillingAuthStatus is ‘failed’.

### actualStatus:

The effective status of the campaign.
Details the reasons why it is not running, if applicable.

### actualStatusString: !

Minimal string representation of the actual status.
One of ‘running’, ‘notRunning’ ,’ended’, ‘paused’, ‘review’, ‘draft’, ‘rejected’ or ‘deleted’.

### updatedDate:

The date this campaign was last updated.

### channel: !

Campaign channel: one of ‘email’, ‘social’ or ‘web’

### isConnectedChannel: !

True if the campaign is run by a third party.

### source: !

The service responsible for the creation of this campaign.

### currency: !

ISO-4217 currency code for the given amount.

### type: !

Type for the campaign. One of “prospecting”, “blended”r
“retargeting”.

### abmType: !

Type of ABM campaign.
Empty string if this is not an ABM campaign.

### targetingType: !

The type of targeting that is used to pick which customers will be reached by this campaign.

### kpiGoal: !

Goal -for the kpiMetric- that drives the campaign’s bid strategy.
Null for automatic.

### kpiCurrency: !

ISO 4217 currency code for kpiGoal.
If not provided assume the currency provided at the Advertisable level.

### kpiMetric: !

Metric being targeted by the campaign’s bid strategy.

### spendLimitUntil:

SpendLimitUntil

### spendLimitUntilReason: !

SpendLimitUntilReason

### processingStatus: !

The processing status of the campaign inside the AdRoll.
It may have a transient value other than “created” while
the campaign is being processed by an internal job.

### billingAuthStatus:

The billing auth status of the campaign inside the AdRoll.
Will default to empty string when API BillingAuthStatus not present.
Result is “failed” when the billing authorization did not complete.

### playbookEID: !

The parent Playbook’s EID for the campaign, only if it exists.

### playbookName: !

The parent Playbook’s Name for the campaign, only if it exists.

### playbookType: !

The parent Playbook’s Type for the campaign, only if it exists.

### inVoltronStrategyEID: !

The EID of this campaign as referenced from its Voltron strategy.
Only available for inventory campaigns of Universal Campaigns.

### proxyStrategyEID: !

The eid of the Proxy Strategy that contains this campaign. Only for Inventory campaigns.

### proxyStrategyIsFrozen: !

The isFrozen value of the Proxy Strategy that contains this campaign. Only for Inventory campaigns.

### proxyStrategyStatus: !

The status of the Proxy Strategy that contains this campaign. Only for Inventory campaigns.

### proxyStrategyName: !

The name of the Proxy Strategy that contains this campaign. Only for Inventory campaigns.

### newsletterScheduled: !

If this is an Email Newsletter campaign, the number of potential recipients.

### newsletterSends: !

If this is an Email Newsletter campaign, the number of emails sent.

### newsletterScheduledDate:

If this is an Email Newsletter campaign, the scheduled date for delivery.
Only if the delivery is scheduled to happen or of it has already occurred. Omitted if in draft, paused or cancelled.

### isBillable: !

True if the campaign is run by NextRoll and will be directly billed to
the advertisable’s account. False if it is run by a third party.

### isFrozen: !

True if the strategy is frozen, and no changes can be made to it.

### syncStatus: !

Only for Connected Campaigns, indicates the status of the sync’ing with the external service.
When available, can be one of “pending”, “synced” or “error”

### syncError: !

Only for Connected Campaigns, shows the error that caused the sync’ing with the external service to fail.
Provided if the syncStatus field is “error”.

### facebookAdsManagerPermalink: !

DEPRECATED: please use adsManagerPermalink instead

### adsManagerPermalink: !

The URL to the campaign if it has been externally connected.

### isIntegrated: !

### useCase: !

### objective: !

The campaign marketing objective returned by AdRoll API.

### funnelStage:

Funnel stage for the campaign. One of “awareness”, “consideration”, “conversion”, or “other”.

### isBudgetBalancingAutomated: !

Indicates if this campaign is a strategy that balances the budget automatically across its inventory campaigns.
False means that inventory campaign budgets are manually set.

### possibleStatusChanges: [!]

Available status changes for the current campaign. BETA.

### performanceTargets: []

PerformanceTargets

### tags: [!]

Internal tags set on creation.

### automationEID:

If managed by an Automation, the EID of the Automation.

### automationNodeEID:

If managed by an Automation,
the EID of the Automation Node that references this entity.

### automationName:

If managed by an Automation, the name of the Automation.

### disabled: !

Indicates if the campaign is disabled.
Currently applies only to Automation-managed campaigns that have been disabled by subscription downgrade action.

### klaviyoFlowEID:

If managed by a Klaviyo Flow, the EID of the Flow.

### klaviyoFlowName:

If managed by a Klaviyo Flow, the name of the Flow.

### CampaignMetricResult

Groups reporting metric data in summary and by date.

**Fields**:

### summary: !

Summarizes the reporting data for the given date range.

### byDate: [!]!

Reporting data by date in the given range.

### byCountry: [!]!

Reporting data by country.

### CampaignQuery

**Fields**:

### byEID(campaign: !):

Obtain a campaign by its unique identifier (EID).

**Arguments**:

### campaign: !

EID of the campaign.

### byEIDs(eids: [!]!): []!

Obtain a list of campaigns by their unique identifiers (EID).

**Arguments**:

### eids: [!]!

List of campaign EIDs.

### byAdvertisable(advertisable: !, isActive: , statuses: [!], excludeStatuses: [!], blacklistStatuses: [!], useCases: [!], types: [!], targetingTypes: [!], abmTypes: [!], channels: [!], sources: [!], funnelStages: [!], objectives: [!], excludeUseCases: [!], excludeTypes: [!], excludeTargetingTypes: [!], excludeABMTypes: [!], excludeChannels: [!], excludeSources: [!], excludeFunnelStages: [!], tagPrefixes: [!]): []!

Obtain a list advertisables owned by an Advertisable.

**Arguments**:

### advertisable: !

The EID of the advertisable whose campaigns are to be fetched

### isActive:

If True, only active campaigns will be returned, and vice versa (Optional; default: True)

### statuses: [!]

Only campaigns that match one of these statuses will be returned (Optional; default: None)

* **Default:**
  [ ]

### excludeStatuses: [!]

Only campaigns whose status is not one of these will be returned (Optional; default: None)

* **Default:**
  [ ]

### blacklistStatuses: [!]

DEPRECATED: please use instead argument excludeStatuses

* **Default:**
  [ ]

### useCases: [!]

Only campaigns that match one of these use cases will be returned (Optional; default: None)

* **Default:**
  [ ]

### types: [!]

Only campaigns that match one of these types will be returned (Optional; default: None)

* **Default:**
  [ ]

### targetingTypes: [!]

Only campaigns that match one of these targeting types will be returned (Optional; default: None)

* **Default:**
  [ ]

### abmTypes: [!]

Only campaigns that match one of these ABM types will be returned. Options: ‘lead_locator’ for Account Targeting, ‘pipeline_accelerator’ for Contact-based. (Optional; default: None)

* **Default:**
  [ ]

### channels: [!]

Only campaigns that match one of these channels will be returned (Optional; default: None)

* **Default:**
  [ ]

### sources: [!]

Only campaigns that match one of these sources will be returned (Optional; default: None)

* **Default:**
  [ ]

### funnelStages: [!]

Only campaigns that match one of these funnel stages will be returned (Optional; default: None)

* **Default:**
  [ ]

### objectives: [!]

Only campaigns that match one of these objectives will be returned (Optional; default: None)

* **Default:**
  [ ]

### excludeUseCases: [!]

Exclude campaigns that match one of the given use cases (Optional; default: None)

* **Default:**
  [ ]

### excludeTypes: [!]

Exclude campaigns that match one of the given types. (Optional; default: None)

* **Default:**
  [ ]

### excludeTargetingTypes: [!]

Exclude campaigns that match one of the given targeting types. (Optional; default: None)

* **Default:**
  [ ]

### excludeABMTypes: [!]

Exclude campaigns that match one of the given ABM types. (Optional; default: None)

* **Default:**
  [ ]

### excludeChannels: [!]

Exclude campaigns that match one of the given channels. (Optional; default: None)

* **Default:**
  [ ]

### excludeSources: [!]

Exclude campaigns that match one of the given sources. (Optional; default: None)

* **Default:**
  [ ]

### excludeFunnelStages: [!]

Exclude campaigns that match one of the given funnel stages. (Optional; default: None)

* **Default:**
  [ ]

### tagPrefixes: [!]

> Only campaigns that have tags that start with one of the given prefixes. (Optional; default: None)
* **Default:**
  [ ]

### byOrganization(organization: !, isActive: , statuses: [!], excludeStatuses: [!], blacklistStatuses: [!], useCases: [!], types: [!], targetingTypes: [!], abmTypes: [!], channels: [!], sources: [!], excludeUseCases: [!], excludeTypes: [!], excludeTargetingTypes: [!], excludeABMTypes: [!], excludeChannels: [!], excludeSources: [!], tagPrefixes: [!]): []!

Obtain a list advertisables owned by an Organization.

**Arguments**:

### organization: !

The EID of the organization whose campaigns are to be fetched

### isActive:

If True, only active campaigns will be returned, and vice versa (Optional; default: True)

### statuses: [!]

Only campaigns that match one of these statuses will be returned (Optional; default: None)

* **Default:**
  [ ]

### excludeStatuses: [!]

Only campaigns whose status is not one of these will be returned (Optional; default: None)

* **Default:**
  [ ]

### blacklistStatuses: [!]

DEPRECATED: please use instead argument excludeStatuses

* **Default:**
  [ ]

### useCases: [!]

Only campaigns that match one of these use cases will be returned (Optional; default: None)

* **Default:**
  [ ]

### types: [!]

Only campaigns that match one of these types will be returned (Optional; default: None)

* **Default:**
  [ ]

### targetingTypes: [!]

Only campaigns that match one of these targeting types will be returned (Optional; default: None)

* **Default:**
  [ ]

### abmTypes: [!]

Only campaigns that match one of these ABM types will be returned. Options: ‘lead_locator’ for Account Targeting, ‘pipeline_accelerator’ for Contact-based. (Optional; default: None)

* **Default:**
  [ ]

### channels: [!]

Only campaigns that match one of these channels will be returned (Optional; default: None)

* **Default:**
  [ ]

### sources: [!]

Only campaigns that match one of these sources will be returned (Optional; default: None)

* **Default:**
  [ ]

### excludeUseCases: [!]

Exclude campaigns that match one of the given use cases (Optional; default: None)

* **Default:**
  [ ]

### excludeTypes: [!]

Exclude campaigns that match one of the given types. (Optional; default: None)

* **Default:**
  [ ]

### excludeTargetingTypes: [!]

Exclude campaigns that match one of the given targeting types. (Optional; default: None)

* **Default:**
  [ ]

### excludeABMTypes: [!]

Exclude campaigns that match one of the given ABM types. (Optional; default: None)

* **Default:**
  [ ]

### excludeChannels: [!]

Exclude campaigns that match one of the given channels. (Optional; default: None)

* **Default:**
  [ ]

### excludeSources: [!]

Exclude campaigns that match one of the given sources. (Optional; default: None)

* **Default:**
  [ ]

### tagPrefixes: [!]

> Only campaigns that have tags that start with one of the given prefixes. (Optional; default: None)
* **Default:**
  [ ]

### metricsTotal:

Provides aggregation for any metrics in the current and child
nodes.

Note that this will not load the metrics by itself, instead it
aggregates loaded metrics fields in its scope.

For details see the documentation of MetricAggregateResult.

### ContextualKeywordTargetingMetrics

**Fields**:

### keywords: [!]!

Labels of the keywords that were targeted.

### impressions: !

The sum of the number of ad impressions.

### clicks: !

The sum of clicks of ads.

### cost: !

Cost associated to ads.

### ctr: !

Click-through rate: The percentage of ad serves that were clicked.
CTR = Clicks / Impressions

### cpm: !

Cost per mille.
Cost per one thousand ad serves on the domain.

CPM ($) = Spend / Impressions \* 1000

### cpc: !

Cost per click: Your average spend for one click.
CPC ($) = Spend / Clicks

### videoImpressions:

Impressions from video ads.

### videoViews:

Number of times the video begun playing.

### videoTwentyFivePercent:

Number of times at least 25% of the video duration was played.

### videoFiftyPercent:

Number of times at least 50% of the video duration was played.

### videoSeventyFivePercent:

Number of times at least 75% of the video duration was played.

### videoHundredPercent:

Number of times the full video duration was played.

### videoCompletionRate:

Video completion rate

Video Completion Rate (x) = Video Viewed To 100% / Video Impressions

### ContextualTargetingResult

Groups reporting metric data in summary and by date format.

**Fields**:

### byKeywords: [!]!

Summarizes by keyword the reporting data for the given date range.

### byTopics: [!]!

Summarizes by topic the reporting data for the given date range.

### ContextualTopicTargetingMetrics

**Fields**:

### topics: [!]!

Labels of the contextual topics that were targeted.

### impressions: !

The sum of the number of ad impressions.

### clicks: !

The sum of clicks of ads.

### cost: !

Cost associated to ads.

### ctr: !

Click-through rate: The percentage of ad serves that were clicked.
CTR = Clicks / Impressions

### cpm: !

Cost per mille.
Cost per one thousand ad serves on the domain.

CPM ($) = Spend / Impressions \* 1000

### cpc: !

Cost per click: Your average spend for one click.
CPC ($) = Spend / Clicks

### videoImpressions:

Impressions from video ads.

### videoViews:

Number of times the video begun playing.

### videoTwentyFivePercent:

Number of times at least 25% of the video duration was played.

### videoFiftyPercent:

Number of times at least 50% of the video duration was played.

### videoSeventyFivePercent:

Number of times at least 75% of the video duration was played.

### videoHundredPercent:

Number of times the full video duration was played.

### videoCompletionRate:

Video completion rate

Video Completion Rate (x) = Video Viewed To 100% / Video Impressions

### ConversionResult

Groups reporting metric data for conversions.

**Fields**:

### byAudience(isActive:) : [!]!

Summarizes by conversion the reporting data for the given date range.

**Arguments**:

### isActive:

If True, only active segments will be returned, and vice versa (Optional; default: False)

### Conversions

Contains reporting metric data for attributions, deliveries

by audience conversion.

**Fields**:

### audienceEID: !

The unique identifier of the audience.

### audienceName: !

The name of the audience.

### audienceDuration: !

The duration in days of the audience.

### audienceIsActive: !

True if the audience is active.

### summary: !

Summarizes the reporting data for the given date range.

### byDate: [!]!

Reporting data by date in the given range.

### impressions:

The sum of the number of ad impressions.

### clicks:

The sum of clicks of all kinds of ads and emails.

### cost:

Cost associated to all kinds of ads and emails.

### conversions:

Conversions
Total.
Conversions (count) = View Conversions + Click Conversions

### clickThroughs:

Click-through conversion (CTC).
A goal completion that happens after someone clicks your ad.

To get the noise from ARA click-throughs, take the square root of araClickThroughsVariance.

### viewThroughs:

View-through conversion (VTC).
A goal completion that happens after someone views your ad, but
does not click.

To get the noise from ARA view-throughs, take the square root of araViewThroughsVariance.

### revenue:

Revenue (amount) = View Revenue + Click Conversions

### clickRevenue:

Click-Attributed Revenue.
Total earnings when someone clicks your ad and converts.

To get the noise from ARA click-throughs, subtract araClickRevenueMin from araClickRevenueMax.

### viewRevenue:

View-Attributed Revenue.
Total earnings when someone views your ad and converts.

To get the noise from ARA view-throughs, subtract araViewRevenueMin from araViewRevenueMax.

### ctr:

Click-through rate.
The percentage of ad serves that were clicked.

CTR (%) = Clicks / Impression \* 100

### cpc:

Cost per click.
Your average spend for one click.

CPC ($) = Spend / Clicks

### cpm:

Cost per mille.
Cost per one thousand ad serves.

CPM ($) = Spend / Impressions \* 1000

### cpa:

Cost per acquisition.
Your average spend per conversion.

CPA ($) = Spend / Conversions

### clickCPA:

Cost-per-click acquisition.
Your average spend for a conversion that happens after someone clicks your ad.

Click CPA ($) = Spend / Click Conversions

### viewCPA:

Cost-per-view acquisition: Your average spend for a
conversion that happens after someone views your ad.

View CPA ($) = Cost / View Throughs

### averageOrderValue:

Average Order Value
Average revenue per attributed conversion.

Average Order Value ($) = Attributed Revenue / Conversions

### ctcRate:

Click-through conversion rate.
The percentage of clicks that resulted in a click-through conversion.

CTC Rate (%) = Click Conversions / Clicks \* 100

### vtcRate:

View-through conversion rate: The percentage of impressions
that resulted in a view-through conversion.

VTC Rate (%) = View Throughs / Impressions \* 100

### roas:

Return on advertising spend: Your profit per dollar spent
on ads.

ROAS (x) = (Click Revenue + View Revenue) / Cost

### clickROAS:

Click return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone clicks
your ad.

Click ROAS (x) = Click Revenue / Cost

### viewROAS:

View return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone views
your ad.

View ROAS (x) = View Revenue / Cost

### roi:

Alias for ‘roas’.

### clickROI:

Alias for ‘clickROAS’.

### viewROI:

Alias for ‘viewROAS’.

### influencedThroughs:

Influenced Conversions.

A conversion touched or assisted by an ad but not attributed due
to the current attribution model.

### influencedRevenue:

Influenced Revenue.

Revenue touched or assisted by an ad but not attributed due to
the current attribution model.

### ConversionsByDate

**Fields**:

### date:

Reporting data by date in the given range.

### impressions:

The sum of the number of ad impressions.

### clicks:

The sum of clicks of all kinds of ads and emails.

### cost:

Cost associated to all kinds of ads and emails.

### conversions:

Conversions
Total.
Conversions (count) = View Conversions + Click Conversions

### clickThroughs:

Click-through conversion (CTC).
A goal completion that happens after someone clicks your ad.

To get the noise from ARA click-throughs, take the square root of araClickThroughsVariance.

### viewThroughs:

View-through conversion (VTC).
A goal completion that happens after someone views your ad, but
does not click.

To get the noise from ARA view-throughs, take the square root of araViewThroughsVariance.

### revenue:

Revenue (amount) = View Revenue + Click Conversions

### clickRevenue:

Click-Attributed Revenue.
Total earnings when someone clicks your ad and converts.

To get the noise from ARA click-throughs, subtract araClickRevenueMin from araClickRevenueMax.

### viewRevenue:

View-Attributed Revenue.
Total earnings when someone views your ad and converts.

To get the noise from ARA view-throughs, subtract araViewRevenueMin from araViewRevenueMax.

### ctr:

Click-through rate.
The percentage of ad serves that were clicked.

CTR (%) = Clicks / Impression \* 100

### cpc:

Cost per click.
Your average spend for one click.

CPC ($) = Spend / Clicks

### cpm:

Cost per mille.
Cost per one thousand ad serves.

CPM ($) = Spend / Impressions \* 1000

### cpa:

Cost per acquisition.
Your average spend per conversion.

CPA ($) = Spend / Conversions

### clickCPA:

Cost-per-click acquisition.
Your average spend for a conversion that happens after someone clicks your ad.

Click CPA ($) = Spend / Click Conversions

### viewCPA:

Cost-per-view acquisition: Your average spend for a
conversion that happens after someone views your ad.

View CPA ($) = Cost / View Throughs

### averageOrderValue:

Average Order Value
Average revenue per attributed conversion.

Average Order Value ($) = Attributed Revenue / Conversions

### ctcRate:

Click-through conversion rate.
The percentage of clicks that resulted in a click-through conversion.

CTC Rate (%) = Click Conversions / Clicks \* 100

### vtcRate:

View-through conversion rate: The percentage of impressions
that resulted in a view-through conversion.

VTC Rate (%) = View Throughs / Impressions \* 100

### roas:

Return on advertising spend: Your profit per dollar spent
on ads.

ROAS (x) = (Click Revenue + View Revenue) / Cost

### clickROAS:

Click return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone clicks
your ad.

Click ROAS (x) = Click Revenue / Cost

### viewROAS:

View return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone views
your ad.

View ROAS (x) = View Revenue / Cost

### roi:

Alias for ‘roas’.

### clickROI:

Alias for ‘clickROAS’.

### viewROI:

Alias for ‘viewROAS’.

### influencedThroughs:

Influenced Conversions.

A conversion touched or assisted by an ad but not attributed due
to the current attribution model.

### influencedRevenue:

Influenced Revenue.

Revenue touched or assisted by an ad but not attributed due to
the current attribution model.

### ConversionsSummary

**Fields**:

### impressions:

The sum of the number of ad impressions.

### clicks:

The sum of clicks of all kinds of ads and emails.

### cost:

Cost associated to all kinds of ads and emails.

### conversions:

Conversions
Total.
Conversions (count) = View Conversions + Click Conversions

### clickThroughs:

Click-through conversion (CTC).
A goal completion that happens after someone clicks your ad.

To get the noise from ARA click-throughs, take the square root of araClickThroughsVariance.

### viewThroughs:

View-through conversion (VTC).
A goal completion that happens after someone views your ad, but
does not click.

To get the noise from ARA view-throughs, take the square root of araViewThroughsVariance.

### revenue:

Revenue (amount) = View Revenue + Click Conversions

### clickRevenue:

Click-Attributed Revenue.
Total earnings when someone clicks your ad and converts.

To get the noise from ARA click-throughs, subtract araClickRevenueMin from araClickRevenueMax.

### viewRevenue:

View-Attributed Revenue.
Total earnings when someone views your ad and converts.

To get the noise from ARA view-throughs, subtract araViewRevenueMin from araViewRevenueMax.

### ctr:

Click-through rate.
The percentage of ad serves that were clicked.

CTR (%) = Clicks / Impression \* 100

### cpc:

Cost per click.
Your average spend for one click.

CPC ($) = Spend / Clicks

### cpm:

Cost per mille.
Cost per one thousand ad serves.

CPM ($) = Spend / Impressions \* 1000

### cpa:

Cost per acquisition.
Your average spend per conversion.

CPA ($) = Spend / Conversions

### clickCPA:

Cost-per-click acquisition.
Your average spend for a conversion that happens after someone clicks your ad.

Click CPA ($) = Spend / Click Conversions

### viewCPA:

Cost-per-view acquisition: Your average spend for a
conversion that happens after someone views your ad.

View CPA ($) = Cost / View Throughs

### averageOrderValue:

Average Order Value
Average revenue per attributed conversion.

Average Order Value ($) = Attributed Revenue / Conversions

### ctcRate:

Click-through conversion rate.
The percentage of clicks that resulted in a click-through conversion.

CTC Rate (%) = Click Conversions / Clicks \* 100

### vtcRate:

View-through conversion rate: The percentage of impressions
that resulted in a view-through conversion.

VTC Rate (%) = View Throughs / Impressions \* 100

### roas:

Return on advertising spend: Your profit per dollar spent
on ads.

ROAS (x) = (Click Revenue + View Revenue) / Cost

### clickROAS:

Click return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone clicks
your ad.

Click ROAS (x) = Click Revenue / Cost

### viewROAS:

View return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone views
your ad.

View ROAS (x) = View Revenue / Cost

### roi:

Alias for ‘roas’.

### clickROI:

Alias for ‘clickROAS’.

### viewROI:

Alias for ‘viewROAS’.

### influencedThroughs:

Influenced Conversions.

A conversion touched or assisted by an ad but not attributed due
to the current attribution model.

### influencedRevenue:

Influenced Revenue.

Revenue touched or assisted by an ad but not attributed due to
the current attribution model.

### Email

**Fields**:

### eid: !

The SendRoll email EID.

### campaign: !

The EID of the AdRoll email campaign who owns this email.

### sequencePosition: !

The position of this email in the campaign’s sequence. (0 for the first email).

### subject: !

The email’s subject.

### name: !

The email’s name.

### status: !

One of ‘running’, ‘scheduled’, ‘ended’, ‘paused’, ‘draft’ or ‘deleted’.

### actualStatus:

The effective status of the campaign.
Details the reasons why it is not running, if applicable.

### actualStatusString: !

Minimal string representation of the actual status.
One of ‘running’, ‘notRunning’ ,’ended’, ‘paused’, ‘draft’ or ‘deleted’.

### delayHours: !

Delay in hours between the previous event in the drip sequence and when this email is scheduled to be sent.

### createdDate:

The date this email was created.

### advertisable: !

Advertisable for this Email.

[WARNING] The advertisable information is not usually available,
so querying this will cause an additional request to be made.

### metrics(start: , end: , pastDays: , currency: , duration:) : !

Metrics for the entity.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The
date range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The
date range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### duration:

[DEPRECATED] Unused.

* **Default:**
  30

### metricsTotal:

Provides aggregation for any metrics in the current and child
nodes.

Note that this will not load the metrics by itself, instead it
aggregates loaded metrics fields in its scope.

For details see the documentation of MetricAggregateResult.

### EmailGroupData

**Fields**:

### eid: !

The SendRoll email EID.

### campaign: !

The EID of the AdRoll email campaign who owns this email.

### sequencePosition: !

The position of this email in the campaign’s sequence. (0 for the first email).

### subject: !

The email’s subject.

### name: !

The email’s name.

### status: !

One of ‘running’, ‘scheduled’, ‘ended’, ‘paused’, ‘draft’ or ‘deleted’.

### actualStatus:

The effective status of the campaign.
Details the reasons why it is not running, if applicable.

### actualStatusString: !

Minimal string representation of the actual status.
One of ‘running’, ‘notRunning’ ,’ended’, ‘paused’, ‘draft’ or ‘deleted’.

### delayHours: !

Delay in hours between the previous event in the drip sequence and when this email is scheduled to be sent.

### createdDate:

The date this email was created.

### advertisable: !

Advertisable for this Email.

[WARNING] The advertisable information is not usually available,
so querying this will cause an additional request to be made.

### EmailQuery

**Fields**:

### byEID(email: !):

Resolves an Email by its EID.

**Arguments**:

### email: !

EID of the Email.

### byEIDs(eids: [!]!): []!

Resolves multiple Emails by their EID.

**Arguments**:

### eids: [!]!

List of Email EIDs.

### byAdvertisable(advertisable: !): []!

Resolves all Emails for an Advertisable.

**Arguments**:

### advertisable: !

The EID of the advertisable whose emails are to be fetched

### byCampaign(campaign: !): []!

Resolves all Emails for a Campaign.

**Arguments**:

### campaign: !

EID of the campaign.

### metricsTotal:

Provides aggregation for any metrics in the current and child
nodes.

Note that this will not load the metrics by itself, instead it
aggregates loaded metrics fields in its scope.

For details see the documentation of MetricAggregateResult.

### FieldAccountMetrics

**Fields**:

### domain:

The domain we show metrics for.

### impressions:

The number of impressions from cookies attached to the domain.

### cost:

Spend against cookies belonging to then domain.

### clicks:

The number of clicks from cookies attached to the domain.

### adjustedViewThroughs:

A goal completion that happens after someone views your ad, but does not click.

### adjustedClickThroughs:

A goal completion that happens after someone clicks your ad.

### adjustedViewRevenue:

Total earnings when someone views your ad and converts.

### adjustedClickRevenue:

Total earnings when someone clicks your ad and converts.

### pageViews:

The number of page views on your site from cookie
attached to the domain (at the advertisable level, not campaigns level)

### engagedVisitors:

The number of unique engaged visitors to your site from cookie
attached to the domain (at the advertisable level, not campaigns level)

### uniqueVisitors:

The number of unique visitors to your site from cookie
attached to the domain (at the advertisable level, not campaigns level)

### lastActivityDate:

Most recent date within the last 30 days for which a cookie attached
to the domain visited your site.

### FieldAccountMetricsSummary

**Fields**:

### summary(start: !, end: !, campaignEIDs: []!, advertisableEID: !, currency:) : []

**Arguments**:

### start: !

### end: !

### campaignEIDs: []!

### advertisableEID: !

### currency:

### FieldConversions

**Fields**:

### conversions(start: , end: , pastDays: , currency:) : !

Metrics for the entity broken down by conversion audiences.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The date
range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The date
range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### FieldGranularConversions

**Fields**:

### granularConversions(start: , end: , pastDays: , currency:) : [!]!

The granular conversions help understand the channels, campaigns, and ads that influence conversions.
Lists the details about a conversion and the data points that determined the decision about its attribution.
Limited to 90 days.

**Arguments**:

### start:

The start date for the conversions period (inclusive).
The date range will be: [start, end)

### end:

The end date for the conversions period (exclusive).
The date range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the conversions in.

* **Default:**
  “USD”

### FieldMetrics

**Fields**:

### metrics(start: , end: , pastDays: , currency: , duration:) : !

Metrics for the entity.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The
date range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The
date range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### duration:

[DEPRECATED] Unused.

* **Default:**
  30

### FieldMetricsForAdvertisable

**Fields**:

### metrics(start: , end: , pastDays: , currency: , duration:) : !

Metrics for the Advertisable.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The
date range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The
date range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### duration:

[DEPRECATED] Unused.

* **Default:**
  30

### FieldMetricsForCampaign

**Fields**:

### metrics(start: , end: , pastDays: , currency: , duration:) : !

Metrics for the Campaign.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The
date range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The
date range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### duration:

[DEPRECATED] Unused.

* **Default:**
  30

### FieldMetricsTotal

**Fields**:

### metricsTotal:

Provides aggregation for any metrics in the current and child
nodes.

Note that this will not load the metrics by itself, instead it
aggregates loaded metrics fields in its scope.

For details see the documentation of MetricAggregateResult.

### FieldUtmBasedConversionsForAdvertisable

**Fields**:

### utmBasedConversions(start: , end: , pastDays: , currency: , model: !): [!]!

UTM based conversions for the Advertisable.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The
date range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The
date range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### model: !

Model can be one of the following:
[utm_firsttouch, utm_lastclick, utm_lasttouch, utm_linear, utm_positional, utm_timedecay]

### FieldsAd

**Fields**:

### eid: !

EID of the ad.

### adFormatID: !

The id of the corresponding ad format in the AdRoll system.

### adFormat: !

Format string. i.e. ‘300 wide x 250 high’.

### adFormatName: !

Format string. i.e. ‘300x250’.

### advertisable: !

The EID of the advertisable to which this ad belongs.

### hasFutureCampaigns: !

Whether or not this ad has the possibility of serving based on the adgroups and campaigns in which it inhabits.

DEPRECATED: this field will stop being supported in the near future.

### destinationURL: !

The URL that the browser will navigate to when this ad is clicked.

### headline: !

For Facebook ads, the text to be displayed as the ad’s headline.

### body: !

For Facebook ads, the text to be displayed as the ad’s body.

### message: !

For Facebook Newsfeed ads, the text to be displayed as the ad’s message.

### callToAction: !

Facebook call to action constant.

### isActive: !

Whether or not this ad is currently active.

### name: !

The name of this ad.

### src: !

This ad’s creative’s source URL.

### previewURL: !

The preview URL for dynamic ads like HTML5.

### status: !

One of ‘running’, ‘paused’, ‘review’, ‘draft’, ‘rejected’, ‘suspended’ or ‘deleted’.

### actualStatus:

The effective status of the campaign.
Details the reasons why it is not running, if applicable.

### actualStatusString: !

Minimal string representation of the actual status. One of ‘running’,
‘notRunning’ ,’ended’, ‘paused’, ‘review’, ‘draft’, ‘rejected’ or ‘deleted’.

### type: !

The ad type: ‘liquid’, ‘image’, ‘flash’ or ‘ad_network’.

### height: !

The height in pixels of this ad’s creative.

### width: !

The width in pixels of this ad’s creative.

### createdDate:

The date this ad was created.

### updatedDate:

The date this ad was last updated.

### hasEdits: !

Whether or not this ad has been edited such that another ad has it’s original ad parameter set to this ad’s EID.

### hasPendingEdits: !

Whether or not this ad has edits that must be reviewed by an AdRoll administrator.

### originalAd: !

The EID of the ad that was edited to create this ad.

### isDynamic: !

Whether or not this is an ad that is dynamically composed when it is served to the user.

### isOutlined: !

Whether or not an outline has been applied to the ad to satisfy network compliancy.

### outlineColor: !

Hexadecimal color code corresponding to the outline of an ad.

### validClicktag: !

If the ad is in flash format, this is the flag showing whether or not the clickTAG is compliant.

### facebookAdsManagerPermalink: !

DEPRECATED: please use adsManagerPermalink instead

### adsManagerPermalink: !

The URL to the ad if it has been externally connected.

### facebookPermalink: !

Facebook permalink if applicable.

### instagramPermalink: !

Instagram permalink if applicable.

### linkedInPermalink: !

LinkedIn permalink if applicable.

### syncStatus: !

Only for Connected Campaigns’ ads, indicates the status of the sync’ing with the external service.
When available, can be one of “pending”, “synced” or “error”

### syncError: !

Only for Connected Campaigns’ ads, shows the error that caused the sync’ing with the external service to fail.
Provided if the syncStatus field is “error”.

### remoteStatus: !

The status of the Ad on the inventory network NextRoll has sync’ed it to (ex: Facebook)

### disapprovalReason: !

The reason why an Ad has been rejected on the inventory network NextRoll has sync’ed it to (ex: Facebook)

### utmSource: !

UTM Source Parameter from this Ad’s destination.

### utmMedium: !

UTM Medium Parameter from this Ad’s destination.

### utmCampaign: !

UTM Campaign Parameter from this Ad’s destination.

### utmTerm: !

UTM Term Parameter from this Ad’s destination.

### utmContent: !

UTM Content Parameter from this Ad’s destination.

### channel: !

The channel for the campaign this ad belongs to. This is only
available when loading the ads through a campaign.

### campaignType: !

The type for the campaign this ad belongs to. This is only
available when loading the ads through a campaign.

### adrollEID: !

The adroll EID for prospecting ads.

### adcrabEID: !

The AdCrab ad EID for this ad (ending in 8ADS).

### inAdgroupEID: !

The AdGroup’s EID in the AdGroupAd relationship, if listed
inside an AdGroup.

### inAdgroupIsActive: !

True of the AdGroupAd relationship is active, if listed inside
an AdGroup.

### inAdgroupStatus: !

The status of the AdGroupAd relationship, if listed inside
an AdGroup.

### inAdgroupRelationshipEID: !

The the internal EID of the AdGroupAd relationship, if such a EID
exists and if the ad is listed inside an AdGroup.

### labels: []!

The list of custom labels to organize and filter the ad.

### labelsString: !

The list of custom labels as String. e.g.: “label1, label2”

### FieldsAdMetrics

**Fields**:

### impressions:

The sum of the number of ad impressions.

### clicks:

The sum of clicks of all kinds of ads and emails.

### cost:

Cost associated to all kinds of ads and emails.

### conversions:

Conversions
Total.
Conversions (count) = View Conversions + Click Conversions

### clickThroughs:

Click-through conversion (CTC).
A goal completion that happens after someone clicks your ad.

To get the noise from ARA click-throughs, take the square root of araClickThroughsVariance.

### viewThroughs:

View-through conversion (VTC).
A goal completion that happens after someone views your ad, but
does not click.

To get the noise from ARA view-throughs, take the square root of araViewThroughsVariance.

### revenue:

Revenue (amount) = View Revenue + Click Conversions

### clickRevenue:

Click-Attributed Revenue.
Total earnings when someone clicks your ad and converts.

To get the noise from ARA click-throughs, subtract araClickRevenueMin from araClickRevenueMax.

### viewRevenue:

View-Attributed Revenue.
Total earnings when someone views your ad and converts.

To get the noise from ARA view-throughs, subtract araViewRevenueMin from araViewRevenueMax.

### ctr:

Click-through rate.
The percentage of ad serves that were clicked.

CTR (%) = Clicks / Impression \* 100

### cpc:

Cost per click.
Your average spend for one click.

CPC ($) = Spend / Clicks

### cpm:

Cost per mille.
Cost per one thousand ad serves.

CPM ($) = Spend / Impressions \* 1000

### cpa:

Cost per acquisition.
Your average spend per conversion.

CPA ($) = Spend / Conversions

### clickCPA:

Cost-per-click acquisition.
Your average spend for a conversion that happens after someone clicks your ad.

Click CPA ($) = Spend / Click Conversions

### viewCPA:

Cost-per-view acquisition: Your average spend for a
conversion that happens after someone views your ad.

View CPA ($) = Cost / View Throughs

### averageOrderValue:

Average Order Value
Average revenue per attributed conversion.

Average Order Value ($) = Attributed Revenue / Conversions

### ctcRate:

Click-through conversion rate.
The percentage of clicks that resulted in a click-through conversion.

CTC Rate (%) = Click Conversions / Clicks \* 100

### vtcRate:

View-through conversion rate: The percentage of impressions
that resulted in a view-through conversion.

VTC Rate (%) = View Throughs / Impressions \* 100

### roas:

Return on advertising spend: Your profit per dollar spent
on ads.

ROAS (x) = (Click Revenue + View Revenue) / Cost

### clickROAS:

Click return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone clicks
your ad.

Click ROAS (x) = Click Revenue / Cost

### viewROAS:

View return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone views
your ad.

View ROAS (x) = View Revenue / Cost

### roi:

Alias for ‘roas’.

### clickROI:

Alias for ‘clickROAS’.

### viewROI:

Alias for ‘viewROAS’.

### FieldsAdgroup

**Fields**:

### eid: !

The EID of the adgroup.

### adOptimization: !

The strategy used to optimize ads when multiple ads fit a single ad space.

### campaign: !

The EID of the campaign that this adgroup is associated with.

### isActive: !

Whether or not this adgroup is currently active.

### name: !

The name of this adgroup.

### status: !

One of ‘approved’, ‘paused’, ‘draft’, ‘rejected’ or ‘deleted’.

### actualStatus:

The effective status of the adgroup.
Details the reasons why it is not running, if applicable.

### actualStatusString: !

Minimal string representation of the actual status. One of
‘running’, ‘notRunning’ ,’ended’, ‘paused’, ‘review’, ‘draft’,
‘rejected’ or ‘deleted’.

### createdDate:

The date this adgroup was created.

### updatedDate:

The date this adgroup was last updated.

### flightTimezone: !

The timezone preference of all flights of this adgroup.

### flights:

Scheduled flight periods when ads will be served. Null if there is no limitation.

### processingStatus: !

The processing status of the campaign inside the AdRoll.
It may have a transient value other than “created” while
the AdGroup is being processed by an internal job.

### significantFlightStartDate:

Start date for the active or most recent flight period in the adgroup.

### significantFlightEndDate:

End date for the active or most recent flight period in the adgroup.

### advertisable: !

Advertisable for this Adgroup. NOTE/FIXME: the advertisable
information is not usually available, so querying this will
cause an additional request to be made.

### kpiGoal:

Goal -for the kpiMetric- that drives the campaign’s bid strategy.
Null for automatic.

### kpiCurrency: !

ISO 4217 currency code for kpiGoal.
If not provided assume the currency provided at the Advertisable level.

### kpiMetric: !

Metric being targeted by the campaign’s bid strategy.

### adType: !

Ad type restriction for this adgroup.
Empty if there is no explicit restriction. Currently one of “static”or “dynamic.

### facebookAdsManagerPermalink: !

DEPRECATED: please use adsManagerPermalink instead

### adsManagerPermalink: !

The URL to the adgroup if it has been externally connected.

### syncStatus: !

Only for Connected Campaigns’ adgroups, indicates the status of the sync’ing with the external service.
When available, can be one of “pending”, “synced” or “error”

### syncError: !

Only for Connected Campaigns’ adgroups, shows the error that caused the sync’ing with the external service to fail.
Provided if the syncStatus field is “error”.

### allowedTargeting: !

The allowed targeting type configured for this adgroup.

### FieldsAdvertisable

**Fields**:

### eid: !

EID of the advertisable.

### isActive: !

Whether or not the advertisable is currently active.

### isB2B: !

Whether or not the advertisable is a B2B customer.
Deprecated field: use businessUnit instead.

### businessUnit: !

The business unit this Advertisable has signed up for.

### isAbmCustomer: !

Whether or not the advertisable is an ABM customer.

### name: !

The name of the advertisable.

### organization: !

The EID of this advertisable’s organization.

### status: !

The status of the advertisable. One of [‘admin_review’, ‘approved’, ‘rejected’, ‘suspended’].

### url: !

The advertisable’s URL.

### currency: !

The currency code (ISO-4217) use by the advertisable’s account.

### clickThroughConversionWindow: !

Duration of this advertisable’s click through conversion window in days.

### viewThroughConversionWindow: !

Duration of this advertisable’s view through conversion window in days.

### createdDate:

The date this advertisable was created.

### revshareViewPercent: !

### revshareClickPercent: !

### FieldsAudience

**Fields**:

### eid: !

The EID of the audience in use.

### segmentEID: !

The EID of the segment describing this audience.

### advertisable: !

The Advertisable for the segment.

### campaign: !

The Campaign for the segment.

### name: !

The Audience Name.

### type: !

The type of the segment. One of:
- “url”: URL
- “crm”: crm
- “pages_viewed”: Pages Viewed
- “products_viewed”: Products Viewed
- “arbitrary_data”: External Data
- “app_install”: App Install
- “facebook_prospecting”: Facebook Prospecting
- “custom”: Partner
- “intent”: Intent
- “impression”: Impression
- “user_attributes”: Attributes
- “user_events”: Events
- “lead_generation”: Lead Generation
- “composite”: Composite
- “event_match”: Event JS Match
- “js_match”: Explicit JS Match
- “ipixel_match”: IPixel Match
- “css_selector”: CSS Selector
- “email_list”: Email List in AdRoll Email.
- “email_domain”: Email Address Domain Match.

### tags: !

Tags explicitly assigned to the segment.

### description: !

Pieces to build the Audience’s description formatted following the type.

### duration: !

The duration of the Audience, in days.

### isActive: !

False if this is segment has been deleted.

### inclusion: !

Is the segment an inclusion segment.

### isConversion: !

True if this is a conversion audience.

### conversionValue: !

The value of a conversion from this segment.

### currency: !

The value of a conversion from this segment. Default to the Advertisable’s currency.

### createdDate:

Date of creation.

### product:

Product the segment belongs to.

### FieldsAudienceMetrics

**Fields**:

### audienceSizeNew:

### audienceSizeTotal:

### FieldsBrandAwarenessForAdvertisables

**Fields**:

### siteBounceRate:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteNewVisitors:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteNewVisitorsNot:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteEngaged:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteEngagedNot:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteEngagedNewVisitors:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteEngagedNewVisitorsNot:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteAddToCart:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteAddToCartNot:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteConverters:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteConvertersNot:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteReturningVisitors:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteReturningVisitorsNot:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### FieldsBrandAwarenessForCampaigns

**Fields**:

### siteBounceRate:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteNewVisitors:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteEngaged:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteEngagedNewVisitors:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteAddToCart:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### FieldsCTVHouseholdMetrics

**Fields**:

### totalUniqueHHsReached:

Number of distinct households that received CTV impressions on a given day

### uniqueHHSiteVisits:

Number of distinct households that visited the site, after viewing an ad

### FieldsCampaign

**Fields**:

### eid: !

EID of the campaign.

### advertisable: !

EID of the advertisable to which this campaign belongs.

### budget: !

The daily budget of the campaign.
Note that this can be an approximation, for example when budgetType = “lifetime” it is:
budget = budgetGoal / numberOfDays(budgetStartDate, budgetEndDate)

### budgetGoal: !

The budget of the campaign, considered for the whole extent of its budgetType.
When budgetType = “lifetime”, it will be applied in the period since budgetStartDate until budgetEndDate.

### budgetType: !

The type of budget of the campaign (daily, lifetime…).
If this includes -auto (i.e. daily-auto), then it is the inventory campaign of a proxy strategy that is auto-balancing the budget for this campaign

### budgetStartDate:

The start date of a lifetime budget.

### budgetEndDate:

The end date of a lifetime budget.

### budgetSettingsString: !

Serialized budget settings as a string.
“budgetType,budgetStartDate,budgetEndDate,budgetGoal”

### createdDate:

The date this campaign was created.

### cpc: !

The CPC for this campaign.

### cpm: !

The CPM for this campaign.

### maxCpm: !

The maximum CPM for this campaign.

### name: !

The name of this campaign.

### startDate:

The day the campaign will start.

### endDate:

The day the campaign will end, exclusive.

### status: !

The status of the campaign.
One of ‘running’, ‘ended’, ‘paused’, ‘review’, ‘draft’, ‘rejected’ or ‘deleted’.
Result is ‘billingFailedPermanent’ or ‘billingFailedRecoverable’ when BillingAuthStatus is ‘failed’.

### actualStatus:

The effective status of the campaign.
Details the reasons why it is not running, if applicable.

### actualStatusString: !

Minimal string representation of the actual status.
One of ‘running’, ‘notRunning’ ,’ended’, ‘paused’, ‘review’, ‘draft’, ‘rejected’ or ‘deleted’.

### updatedDate:

The date this campaign was last updated.

### channel: !

Campaign channel: one of ‘email’, ‘social’ or ‘web’

### isConnectedChannel: !

True if the campaign is run by a third party.

### source: !

The service responsible for the creation of this campaign.

### currency: !

ISO-4217 currency code for the given amount.

### type: !

Type for the campaign. One of “prospecting”, “blended”r
“retargeting”.

### abmType: !

Type of ABM campaign.
Empty string if this is not an ABM campaign.

### targetingType: !

The type of targeting that is used to pick which customers will be reached by this campaign.

### kpiGoal: !

Goal -for the kpiMetric- that drives the campaign’s bid strategy.
Null for automatic.

### kpiCurrency: !

ISO 4217 currency code for kpiGoal.
If not provided assume the currency provided at the Advertisable level.

### kpiMetric: !

Metric being targeted by the campaign’s bid strategy.

### spendLimitUntil:

SpendLimitUntil

### spendLimitUntilReason: !

SpendLimitUntilReason

### processingStatus: !

The processing status of the campaign inside the AdRoll.
It may have a transient value other than “created” while
the campaign is being processed by an internal job.

### billingAuthStatus:

The billing auth status of the campaign inside the AdRoll.
Will default to empty string when API BillingAuthStatus not present.
Result is “failed” when the billing authorization did not complete.

### playbookEID: !

The parent Playbook’s EID for the campaign, only if it exists.

### playbookName: !

The parent Playbook’s Name for the campaign, only if it exists.

### playbookType: !

The parent Playbook’s Type for the campaign, only if it exists.

### inVoltronStrategyEID: !

The EID of this campaign as referenced from its Voltron strategy.
Only available for inventory campaigns of Universal Campaigns.

### proxyStrategyEID: !

The eid of the Proxy Strategy that contains this campaign. Only for Inventory campaigns.

### proxyStrategyIsFrozen: !

The isFrozen value of the Proxy Strategy that contains this campaign. Only for Inventory campaigns.

### proxyStrategyStatus: !

The status of the Proxy Strategy that contains this campaign. Only for Inventory campaigns.

### proxyStrategyName: !

The name of the Proxy Strategy that contains this campaign. Only for Inventory campaigns.

### newsletterScheduled: !

If this is an Email Newsletter campaign, the number of potential recipients.

### newsletterSends: !

If this is an Email Newsletter campaign, the number of emails sent.

### newsletterScheduledDate:

If this is an Email Newsletter campaign, the scheduled date for delivery.
Only if the delivery is scheduled to happen or of it has already occurred. Omitted if in draft, paused or cancelled.

### isBillable: !

True if the campaign is run by NextRoll and will be directly billed to
the advertisable’s account. False if it is run by a third party.

### isFrozen: !

True if the strategy is frozen, and no changes can be made to it.

### syncStatus: !

Only for Connected Campaigns, indicates the status of the sync’ing with the external service.
When available, can be one of “pending”, “synced” or “error”

### syncError: !

Only for Connected Campaigns, shows the error that caused the sync’ing with the external service to fail.
Provided if the syncStatus field is “error”.

### facebookAdsManagerPermalink: !

DEPRECATED: please use adsManagerPermalink instead

### adsManagerPermalink: !

The URL to the campaign if it has been externally connected.

### isIntegrated: !

### useCase: !

### objective: !

The campaign marketing objective returned by AdRoll API.

### funnelStage:

Funnel stage for the campaign. One of “awareness”, “consideration”, “conversion”, or “other”.

### isBudgetBalancingAutomated: !

Indicates if this campaign is a strategy that balances the budget automatically across its inventory campaigns.
False means that inventory campaign budgets are manually set.

### possibleStatusChanges: [!]

Available status changes for the current campaign. BETA.

### performanceTargets: []

PerformanceTargets

### tags: [!]

Internal tags set on creation.

### automationEID:

If managed by an Automation, the EID of the Automation.

### automationNodeEID:

If managed by an Automation,
the EID of the Automation Node that references this entity.

### automationName:

If managed by an Automation, the name of the Automation.

### disabled: !

Indicates if the campaign is disabled.
Currently applies only to Automation-managed campaigns that have been disabled by subscription downgrade action.

### klaviyoFlowEID:

If managed by a Klaviyo Flow, the EID of the Flow.

### klaviyoFlowName:

If managed by a Klaviyo Flow, the name of the Flow.

### FieldsCustomMetrics

**Fields**:

### customMetric(formula:) : !

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Usage:
- Operators: ‘+’, ‘-’, ‘\*’, ‘/’ and parentheses () are valid
Requires formula to have space-seperated operand and operators.

e.g. costPerImpression: customMetric(formula: “cost / impressions”)

**Arguments**:

### formula:

### FieldsEmail

**Fields**:

### eid: !

The SendRoll email EID.

### campaign: !

The EID of the AdRoll email campaign who owns this email.

### sequencePosition: !

The position of this email in the campaign’s sequence. (0 for the first email).

### subject: !

The email’s subject.

### name: !

The email’s name.

### status: !

One of ‘running’, ‘scheduled’, ‘ended’, ‘paused’, ‘draft’ or ‘deleted’.

### actualStatus:

The effective status of the campaign.
Details the reasons why it is not running, if applicable.

### actualStatusString: !

Minimal string representation of the actual status.
One of ‘running’, ‘notRunning’ ,’ended’, ‘paused’, ‘draft’ or ‘deleted’.

### delayHours: !

Delay in hours between the previous event in the drip sequence and when this email is scheduled to be sent.

### createdDate:

The date this email was created.

### advertisable: !

Advertisable for this Email.

[WARNING] The advertisable information is not usually available,
so querying this will cause an additional request to be made.

### FieldsEmailMetrics

**Fields**:

### sends:

Number of emails sent by a campaign.

### opens:

Number of unique-by-session email opens collected for a
campaign.

WARNING: this field is deprecated, please use “emailUniqueOpen” instead. To ease up
the transition this field will still be available, but always return null.

### openRate:

WARNING: this field is deprecated, please use “emailUniqueOpenRate”.
To ease up the transition this field will still be available, but always return null.

### emailScheduled: !

Total emails scheduled to be sent as part if this campaign.

### emailSentUnconfirmed: !

Total emails attempted to be sent.

### emailBounced: !

Deliveries that were rejected by the recipient's email service provider.

### emailSentConfirmed: !

Total emails confirmed to have been sent by the Email Service Provider.

### emailDeliveryRate: !

The percent of emails that have been confirmed to be delivered, over the send attempts.

### emailMarkedSpam: !

Recipients who report your emails as spam.

### emailUniqueMarkedSpam: !

Recipients who report your emails as spam, uniqued.

### emailUniqueOpen: !

When an email is opened by a user in its lifetime.

### emailUniqueOpenRate: !

The percent of sent emails that are opened once in a user's lifetime.

### emailUniqueClick: !

The number of times a link in an email was clicked once in a user's lifetime.

### emailUniqueClickRate: !

The percentage of emails opened that were clicked once in a user's lifetime.

### emailUniqueUnsubscribers: !

Recipients that unsubscribe from the email list, uniqued.

### emailUniqueUnsubscribeRate: !

The percent of recipients that have unsubscribers (unique) over the number of confirmed to be deliveries.

### emailUnsubscribers: !

Recipients that unsubscribe from the email list

### emailUniqueClicksByCountry:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times an email was clicked once in a user's lifetime broken out by ISO-2 country code

### emailUniqueOpensByCountry:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times an email is opened by a user in its lifetime, broken out by ISO-2 country code

### emailUniqueClicksByDeviceType:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times a link in an email was clicked once in a user's lifetime, broken out by device type
One of ‘pc’, ‘mobile’, ‘tablet’, ‘other’.

### emailUniqueOpensByDeviceType:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times an email is opened by a user in its lifetime, broken out by device type
One of ‘pc’, ‘mobile’, ‘tablet’, ‘other’.

### emailUniqueClicksByXpathUrl:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Unique clicks by xpath;url present in an email message
The key <xpath>;<url or macro> consists in 2 parts:
1. A XPath locator to the individual element that was clicked in the email message, based on a HTML5-compliant tree.
2. URL or macro: either a static URL that was clicked present in the email template or, the macro used to generate the URL. Eg.: {{product.url}}. Useful to identify links generated for the same intent, but it might show differently for emailed contacts.

In the future we may break this out to seperate metrics

### FieldsForUtmBasedConversions

**Fields**:

### utm: !

### aov: !

### assistConversions: !

### assistRevenue: !

### assistAov: !

### conversions: !

### revenue: !

### FieldsInfluencedAttributionMetrics

**Fields**:

### influencedThroughs:

Influenced Conversions.

A conversion touched or assisted by an ad but not attributed due
to the current attribution model.

### influencedRevenue:

Influenced Revenue.

Revenue touched or assisted by an ad but not attributed due to
the current attribution model.

### FieldsOrganization

**Fields**:

### eid: !

EID of the organization.

### name: !

Name of the organization.

### createdDate:

Created date for the organization.

### FieldsProspectingMetrics

**Fields**:

### newVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyNewVisitors instead.

The number of unique new visitors who came to your site after
viewing a prospecting ad.

### engagedVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyEngagedVisitors instead.

The number of unique new visitors who have viewed at least 3 pages
on your site after viewing a prospecting ad.

### bouncedVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL.

Visitors who have only viewed one page and left your site
after viewing a prospecting ad.

### nonBouncedVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL.

Visitors who have only viewed more than one page after
viewing a prospecting ad.

### newVisitorCost:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyNewVisitorCost instead.

The cost for each unique new visitor that came to your site after
viewing a prospecting ad.

New Visitor Cost = cost / newVisitors

### engagedVisitorCost:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyEngagedVisitorCost instead.

The cost for each unique new visitor that has viewed at least 3
pages on your site after viewing a prospecting ad

Engaged Visitor Cost = cost / engagedVisitors

### bounceRate:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL.

The percentage of new visitors who have only viewed one page
and left your site after viewing a prospecting ad.

Bounce Rate (%) = bouncedVisitors / newVisitors \* 100.

### dailyNewVisitors:

The number of daily new visitors who came to your site after
viewing a prospecting ad.

### dailyReturnVisitors:

The number of daily new visitors who return to your site after
viewing a prospecting ad.

### dailyEngagedVisitors:

The number of daily new visitors who have viewed at least 3 pages
on your site after viewing a prospecting ad.

### dailyBounceRate:

The percentage of daily new visitors who have only viewed one page
and left your site after viewing a prospecting ad.

### dailyNewVisitorCost:

The cost for each daily new visitor that came to your site after
viewing a prospecting ad.

New Visitor Cost = cost / dailyNewVisitors

### dailyEngagedVisitorCost:

The cost for each daily new visitor that has viewed at least 3
pages on your site after viewing a prospecting ad

Engaged Visitor Cost = cost / dailyEngagedVisitors

### FieldsReachFrequencyMetrics

**Fields**:

### convCountImpRate01: !

Number of converters who saw an average of 0-1 ads/day in the last 30 days.

### convCountImpRate12: !

Number of converters who saw an average of 1-2 ads/day in the last 30 days.

### convCountImpRate23: !

Number of converters who saw an average of 2-3 ads/day in the last 30 days.

### convCountImpRate34: !

Number of converters who saw an average of 3-4 ads/day in the last 30 days.

### convCountImpRate4: !

Number of converters who saw an average of 4+ ads/day in the last 30 days.

### nonConvCountImpRate01: !

Number of non-converters who saw an average of 0-1 ads/day in the last 30 days.

### nonConvCountImpRate12: !

Number of non-converters who saw an average of 1-2 ads/day in the last 30 days.

### nonConvCountImpRate23: !

Number of non-converters who saw an average of 2-3 ads/day in the last 30 days.

### nonConvCountImpRate34: !

Number of non-converters who saw an average of 3-4 ads/day in the last 30 days.

### nonConvCountImpRate4: !

Number of non-converters who saw an average of 4+ ads/day in the last 30 days.

### FieldsReachMetrics

**Fields**:

### frequency: !

Number of ads seen per day by reached users (only applies to WEB campaigns)

Frequency = total impressions/reached users

### deviceFrequency: !

Number of ads seen per day by reached devices (only applies to CTV campaigns)

Device Frequency = total impressions/reached devices

### FieldsSMSMetrics

**Fields**:

### smsSentDelivered: !

Total number of SMS messages that were delivered (and confirmed by the recipient)

### smsClicks: !

Total number of times that a link in the SMS message was clicked.

### FieldsSegment

**Fields**:

### eid: !

The Segment EID.

### name: !

The Segment Name.

### duration: !

The Segment’s duration in days.

### isActive: !

False if the segment has been deleted.

### isConversion: !

True if this is a conversion segment.

### type: !

Segment type.

### tags: !

Tags explicitly assigned to the segment.

### conversionValue: !

The value of a conversion from this segment.

### currency: !

The value of a conversion from this segment. Default to the
Advertisable’s currency.

### description: !

Pieces to build the Segment’s description formatted following the type.

### product:

Product the segment belongs to.

### FieldsVideoMetrics

**Fields**:

### videoImpressions:

Impressions from video ads.

### videoViews:

Number of times the video begun playing.

### videoTwentyFivePercent:

Number of times at least 25% of the video duration was played.

### videoFiftyPercent:

Number of times at least 50% of the video duration was played.

### videoSeventyFivePercent:

Number of times at least 75% of the video duration was played.

### videoHundredPercent:

Number of times the full video duration was played.

### videoCompletionRate:

Video completion rate

Video Completion Rate (x) = Video Viewed To 100% / Video Impressions

### GranularConversion

A row describing a granular conversion.

**Fields**:

### time:

When the conversion happened.

### type: !

There are two types of conversions: “Click through” (CTC), “View through” (VTC) or “Influenced”.

### attributionModel: !

The attribution model applied at the time of conversion.

### attributionCredit: !

The type of credit assigned: “attributed” or “influenced”.

### adrollConversionId: !

The unique identifier for the attributed or influenced conversion.

### touchpointTimestamp:

The last preceding AdRoll touchpoint, such as an impression or click.

### attributedConversions: !

The number of conversions attributed to your AdRoll ads based on your selected attribution model.
If the impression or click is attributed the conversion, the value will be 1.
If the impression or click influenced the conversion, the value will be 0.

### lastTouchAttribution: !

True if it has been attributed as last touch.

### channel: !

The channel that served the converting ad (Web, Facebook, Email).

### campaignEID: !

The EID of the campaign that served the converting ad.

### campaignType: !

The type of the campaign that served the converting ad. (Deprecated)

### campaignAbmType: !

The type for RollWorks ABM campaigns.

### campaignTargetingType: !

The targeting type of the campaign that served the converting ad.

### campaignName: !

The name of the campaign that served the converting ad.

### adgroupEID: !

The EID of the AdGroup that served the converting ad.

### adgroupName: !

The name of the AdGroup that served the converting ad.

### adEID: !

The EID of the ad that resulted in a conversion.

### adName: !

The name of the ad that resulted in a conversion.

### adSize: !

Size of the converting ad.

### segmentEID: !

The EID of the associated conversion audience.

### segmentName: !

The name of the associated conversion audience.

### playbookEID: !

The associated Playbook’s EID or empty string if not applicable.

### playbookName: !

The associated Playbook’s Name or empty string if not applicable.

### playbookType: !

The associated Playbook’s Type or empty string if not applicable.

### attributedRevenue: !

Revenue for the attributed conversions
(only populates if you either specify a fixed conversion value
or have [enhanced conversion tracking]([https://help.adroll.com/hc/en-us/articles/212629938](https://help.adroll.com/hc/en-us/articles/212629938)) set up).

### externalData:

Data recorded by the AdRoll Pixel on the conversion event.

### device: !

If available the device where the conversion happened.

### country: !

If available (provided by the network, unavailable on Facebook):
the country where the conversion happened.

### city: !

If available (provided by the network, unavailable on Facebook):
the city where the conversion happened.

### firstTouchTimestamp:

When the first AdRoll touch occurred.

### lastTouchTimestamp:

When the final AdRoll touch occurred.

### daysToConversionFirstTouch: !

Time from first AdRoll touch to conversion (days).

### daysToConversionLastTouch: !

Time from last AdRoll touch to conversion (days).

### referrerURL: !

URL preceding the conversion.

### cookie: !

The AdRoll cookie that was used to track this conversion’s journey.
This field is for internal use only, it will always return an empty string for external users.

### GroupListRow

[BETA] This GraphQL node is currently under development.

Avoid its use in production until it has passed some thorough QA.

Row returned for each row in a group by query from

‘group.loadByList’.

The available data depends on the arguments to the group by:

- Entity data is only available when grouping by entity and

only for the entity being grouped by.

- Date is only available when grouping by date.
- Only columns specified in the group by are available for a

particular group.

Groups are returned as a flat list but should be interpret as a

hierarchy:

- There is always one ‘root’ group that has no entity data. The

metrics in this root group are the total aggregate.

- Children groups have a ‘parentId’ field that is the ‘id’ of

their parent (e.g. children of the root group will have a

parentId of ‘root’).

- The final level of groups in the query have the ‘leaf’ field

as true. This is made for easy filtering when only the leaf

nodes are required.

- Each group in the ‘groups’ parameter for the query creates

a level of sub-groups in order. So the first group parameter

will correspond to children of the ‘root’ group, while the

last group parameter will correspond to the ‘leaf’ groups.

**Fields**:

### id: !

Unique ID for this group.

### parentId: !

The unique ID of the parent group. Empty for the root group.

### leaf: !

Leaf is true for the leaf groups (groups with no children).
This corresponds to the last ‘groups’ parameter in the GroupBy.

### date: !

When grouping by date, this is the metric date for this
group. The format depends on the ‘date’ argument of the
GroupBy:

- day:       “2018-12-30”
- week:      “2018-W52”
- month:     “2018-12”
- year:      “2018”
- dayofweek: “sun”

### dateKey: !

This is a sortable value for the ‘date’ argument. It is
equal to ‘date’ except for when using ‘dayofweek’ when it is
the number corresponding to the week day order.

### domain: !

When grouping by domain, this returns the domain for the
current group.

### columns: !

When grouping by columns, this will return a JSON object
whose keys are the group column names (as specified in the
GroupBy argument) and the values are the column values for
the current group.

### organization:

Organization data for the group. This is only available when
grouping by organizations (e.g. ‘entity’ = ‘organization’).

### advertisable:

Advertisable data for the group. This is only available when
grouping by advertisables (e.g. ‘entity’ = ‘advertisable’).

### campaign:

Campaign data for the group. This is only available when
grouping by campaigns (e.g. ‘entity’ = ‘campaign’).

### adgroup:

Adgroup data for the group. This is only available when
grouping by adgroups (e.g. ‘entity’ = ‘adgroup’).

### ad:

Ad data for the group. This is only available when
grouping by ads (e.g. ‘entity’ = ‘ad’).

### segment:

Segment data for the group. This is only available when
grouping by segments (e.g. ‘entity’ = ‘segment’).

### email:

Email data for the group. This is only available when
grouping by emails (e.g. ‘entity’ = ‘email’).

### audience:

Audience data for the group. This is only available when
grouping by audiences (e.g. ‘entity’ = ‘audience’).

### impressions:

The sum of the number of ad impressions.

### clicks:

The sum of clicks of all kinds of ads and emails.

### cost:

Cost associated to all kinds of ads and emails.

### conversions:

Conversions
Total.
Conversions (count) = View Conversions + Click Conversions

### clickThroughs:

Click-through conversion (CTC).
A goal completion that happens after someone clicks your ad.

To get the noise from ARA click-throughs, take the square root of araClickThroughsVariance.

### viewThroughs:

View-through conversion (VTC).
A goal completion that happens after someone views your ad, but
does not click.

To get the noise from ARA view-throughs, take the square root of araViewThroughsVariance.

### revenue:

Revenue (amount) = View Revenue + Click Conversions

### clickRevenue:

Click-Attributed Revenue.
Total earnings when someone clicks your ad and converts.

To get the noise from ARA click-throughs, subtract araClickRevenueMin from araClickRevenueMax.

### viewRevenue:

View-Attributed Revenue.
Total earnings when someone views your ad and converts.

To get the noise from ARA view-throughs, subtract araViewRevenueMin from araViewRevenueMax.

### ctr:

Click-through rate.
The percentage of ad serves that were clicked.

CTR (%) = Clicks / Impression \* 100

### cpc:

Cost per click.
Your average spend for one click.

CPC ($) = Spend / Clicks

### cpm:

Cost per mille.
Cost per one thousand ad serves.

CPM ($) = Spend / Impressions \* 1000

### cpa:

Cost per acquisition.
Your average spend per conversion.

CPA ($) = Spend / Conversions

### clickCPA:

Cost-per-click acquisition.
Your average spend for a conversion that happens after someone clicks your ad.

Click CPA ($) = Spend / Click Conversions

### viewCPA:

Cost-per-view acquisition: Your average spend for a
conversion that happens after someone views your ad.

View CPA ($) = Cost / View Throughs

### averageOrderValue:

Average Order Value
Average revenue per attributed conversion.

Average Order Value ($) = Attributed Revenue / Conversions

### ctcRate:

Click-through conversion rate.
The percentage of clicks that resulted in a click-through conversion.

CTC Rate (%) = Click Conversions / Clicks \* 100

### vtcRate:

View-through conversion rate: The percentage of impressions
that resulted in a view-through conversion.

VTC Rate (%) = View Throughs / Impressions \* 100

### roas:

Return on advertising spend: Your profit per dollar spent
on ads.

ROAS (x) = (Click Revenue + View Revenue) / Cost

### clickROAS:

Click return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone clicks
your ad.

Click ROAS (x) = Click Revenue / Cost

### viewROAS:

View return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone views
your ad.

View ROAS (x) = View Revenue / Cost

### roi:

Alias for ‘roas’.

### clickROI:

Alias for ‘clickROAS’.

### viewROI:

Alias for ‘viewROAS’.

### influencedThroughs:

Influenced Conversions.

A conversion touched or assisted by an ad but not attributed due
to the current attribution model.

### influencedRevenue:

Influenced Revenue.

Revenue touched or assisted by an ad but not attributed due to
the current attribution model.

### audienceSizeNew:

### audienceSizeTotal:

### newVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyNewVisitors instead.

The number of unique new visitors who came to your site after
viewing a prospecting ad.

### engagedVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyEngagedVisitors instead.

The number of unique new visitors who have viewed at least 3 pages
on your site after viewing a prospecting ad.

### bouncedVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL.

Visitors who have only viewed one page and left your site
after viewing a prospecting ad.

### nonBouncedVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL.

Visitors who have only viewed more than one page after
viewing a prospecting ad.

### newVisitorCost:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyNewVisitorCost instead.

The cost for each unique new visitor that came to your site after
viewing a prospecting ad.

New Visitor Cost = cost / newVisitors

### engagedVisitorCost:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyEngagedVisitorCost instead.

The cost for each unique new visitor that has viewed at least 3
pages on your site after viewing a prospecting ad

Engaged Visitor Cost = cost / engagedVisitors

### bounceRate:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL.

The percentage of new visitors who have only viewed one page
and left your site after viewing a prospecting ad.

Bounce Rate (%) = bouncedVisitors / newVisitors \* 100.

### dailyNewVisitors:

The number of daily new visitors who came to your site after
viewing a prospecting ad.

### dailyReturnVisitors:

The number of daily new visitors who return to your site after
viewing a prospecting ad.

### dailyEngagedVisitors:

The number of daily new visitors who have viewed at least 3 pages
on your site after viewing a prospecting ad.

### dailyBounceRate:

The percentage of daily new visitors who have only viewed one page
and left your site after viewing a prospecting ad.

### dailyNewVisitorCost:

The cost for each daily new visitor that came to your site after
viewing a prospecting ad.

New Visitor Cost = cost / dailyNewVisitors

### dailyEngagedVisitorCost:

The cost for each daily new visitor that has viewed at least 3
pages on your site after viewing a prospecting ad

Engaged Visitor Cost = cost / dailyEngagedVisitors

### sends:

Number of emails sent by a campaign.

### opens:

Number of unique-by-session email opens collected for a
campaign.

WARNING: this field is deprecated, please use “emailUniqueOpen” instead. To ease up
the transition this field will still be available, but always return null.

### openRate:

WARNING: this field is deprecated, please use “emailUniqueOpenRate”.
To ease up the transition this field will still be available, but always return null.

### emailScheduled: !

Total emails scheduled to be sent as part if this campaign.

### emailSentUnconfirmed: !

Total emails attempted to be sent.

### emailBounced: !

Deliveries that were rejected by the recipient's email service provider.

### emailSentConfirmed: !

Total emails confirmed to have been sent by the Email Service Provider.

### emailDeliveryRate: !

The percent of emails that have been confirmed to be delivered, over the send attempts.

### emailMarkedSpam: !

Recipients who report your emails as spam.

### emailUniqueMarkedSpam: !

Recipients who report your emails as spam, uniqued.

### emailUniqueOpen: !

When an email is opened by a user in its lifetime.

### emailUniqueOpenRate: !

The percent of sent emails that are opened once in a user's lifetime.

### emailUniqueClick: !

The number of times a link in an email was clicked once in a user's lifetime.

### emailUniqueClickRate: !

The percentage of emails opened that were clicked once in a user's lifetime.

### emailUniqueUnsubscribers: !

Recipients that unsubscribe from the email list, uniqued.

### emailUniqueUnsubscribeRate: !

The percent of recipients that have unsubscribers (unique) over the number of confirmed to be deliveries.

### emailUnsubscribers: !

Recipients that unsubscribe from the email list

### emailUniqueClicksByCountry:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times an email was clicked once in a user's lifetime broken out by ISO-2 country code

### emailUniqueOpensByCountry:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times an email is opened by a user in its lifetime, broken out by ISO-2 country code

### emailUniqueClicksByDeviceType:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times a link in an email was clicked once in a user's lifetime, broken out by device type
One of ‘pc’, ‘mobile’, ‘tablet’, ‘other’.

### emailUniqueOpensByDeviceType:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times an email is opened by a user in its lifetime, broken out by device type
One of ‘pc’, ‘mobile’, ‘tablet’, ‘other’.

### emailUniqueClicksByXpathUrl:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Unique clicks by xpath;url present in an email message
The key <xpath>;<url or macro> consists in 2 parts:
1. A XPath locator to the individual element that was clicked in the email message, based on a HTML5-compliant tree.
2. URL or macro: either a static URL that was clicked present in the email template or, the macro used to generate the URL. Eg.: {{product.url}}. Useful to identify links generated for the same intent, but it might show differently for emailed contacts.

In the future we may break this out to seperate metrics

### smsSentDelivered: !

Total number of SMS messages that were delivered (and confirmed by the recipient)

### smsClicks: !

Total number of times that a link in the SMS message was clicked.

### videoImpressions:

Impressions from video ads.

### videoViews:

Number of times the video begun playing.

### videoTwentyFivePercent:

Number of times at least 25% of the video duration was played.

### videoFiftyPercent:

Number of times at least 50% of the video duration was played.

### videoSeventyFivePercent:

Number of times at least 75% of the video duration was played.

### videoHundredPercent:

Number of times the full video duration was played.

### videoCompletionRate:

Video completion rate

Video Completion Rate (x) = Video Viewed To 100% / Video Impressions

### siteBounceRate:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteNewVisitors:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteNewVisitorsNot:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteEngaged:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteEngagedNot:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteEngagedNewVisitors:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteEngagedNewVisitorsNot:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteAddToCart:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteAddToCartNot:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteConverters:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteConvertersNot:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteReturningVisitors:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteReturningVisitorsNot:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### GroupQuery

[BETA] This GraphQL node is currently under development.

Avoid its use in production until it has passed some thorough QA.

Provides arbitrary grouping for queries.

**Fields**:

### loadBy(eids: [!]!, by: !, start: , end: , pastDays: , currency: , groups: [!]!):

Loads entities and metrics providing for arbitrary grouping.

Each group in the ‘groups’ argument will create a group
level in the hierarchy. The first root group will always be
empty and can be used as an aggregate for all the metrics.

**Arguments**:

### eids: [!]!

List of EIDs to load by. The kind of entity being loaded
by is specified with the ‘by’ argument.

### by: !

Kind of entity to load by. The EIDs of the entities to
load by are specified in the ‘eids’ argument.

### start:

The start date for the metrics period (inclusive).
The date range will be: [start, end)

### end:

The end date for the metrics period (exclusive).
The date range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### groups: [!]!

List of groups to group by.

* **Default:**
  [ ]

### loadByList(eids: [!]!, by: !, start: , end: , pastDays: , currency: , groups: [!]!): [!]!

Loads entities and metrics providing for arbitrary grouping.

This differs from loadBy in that the group hierarchy is
returned as a flat list that must be reconstructed as a
tree by the client.

For details on how the group hierarchy is returned, see the
documentation for GroupListRow.

**Arguments**:

### eids: [!]!

List of EIDs to load by. The kind of entity being loaded
by is specified with the ‘by’ argument.

### by: !

Kind of entity to load by. The EIDs of the entities to
load by are specified in the ‘eids’ argument.

### start:

The start date for the metrics period (inclusive).
The date range will be: [start, end)

### end:

The end date for the metrics period (exclusive).
The date range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### groups: [!]!

List of groups to group by.

* **Default:**
  [ ]

### GroupResult

[BETA] This GraphQL node is currently under development.

Avoid its use in production until it has passed some thorough QA.

Result for the ‘groups.loadBy’ field.

**Fields**:

### id: !

Unique ID for this group.

### groups: [!]!

Return children groups if available.

### date: !

When grouping by date, this is the metric date for this
group. The format depends on the ‘date’ argument of the
GroupBy:

- day:       “2018-12-30”
- week:      “2018-W52”
- month:     “2018-12”
- year:      “2018”
- dayofweek: “sun”

### dateKey: !

This is a sortable value for the ‘date’ argument. It is
equal to ‘date’ except for when using ‘dayofweek’ when it is
the number corresponding to the week day order.

### domain: !

When grouping by domain, this returns the domain for the
current group.

### columns: !

When grouping by columns, this will return a JSON object
whose keys are the group column names (as specified in the
GroupBy argument) and the values are the column values for
the current group.

### organization:

Organization data for the group. This is only available when
grouping by organizations (e.g. ‘entity’ = ‘organization’).

### advertisable:

Advertisable data for the group. This is only available when
grouping by advertisables (e.g. ‘entity’ = ‘advertisable’).

### campaign:

Campaign data for the group. This is only available when
grouping by campaigns (e.g. ‘entity’ = ‘campaign’).

### adgroup:

Adgroup data for the group. This is only available when
grouping by adgroups (e.g. ‘entity’ = ‘adgroup’).

### ad:

Ad data for the group. This is only available when
grouping by ads (e.g. ‘entity’ = ‘ad’).

### segment:

Segment data for the group. This is only available when
grouping by segments (e.g. ‘entity’ = ‘segment’).

### email:

Email data for the group. This is only available when
grouping by emails (e.g. ‘entity’ = ‘email’).

### audience:

Audience data for the group. This is only available when
grouping by audiences (e.g. ‘entity’ = ‘audience’).

### impressions:

The sum of the number of ad impressions.

### clicks:

The sum of clicks of all kinds of ads and emails.

### cost:

Cost associated to all kinds of ads and emails.

### conversions:

Conversions
Total.
Conversions (count) = View Conversions + Click Conversions

### clickThroughs:

Click-through conversion (CTC).
A goal completion that happens after someone clicks your ad.

To get the noise from ARA click-throughs, take the square root of araClickThroughsVariance.

### viewThroughs:

View-through conversion (VTC).
A goal completion that happens after someone views your ad, but
does not click.

To get the noise from ARA view-throughs, take the square root of araViewThroughsVariance.

### revenue:

Revenue (amount) = View Revenue + Click Conversions

### clickRevenue:

Click-Attributed Revenue.
Total earnings when someone clicks your ad and converts.

To get the noise from ARA click-throughs, subtract araClickRevenueMin from araClickRevenueMax.

### viewRevenue:

View-Attributed Revenue.
Total earnings when someone views your ad and converts.

To get the noise from ARA view-throughs, subtract araViewRevenueMin from araViewRevenueMax.

### ctr:

Click-through rate.
The percentage of ad serves that were clicked.

CTR (%) = Clicks / Impression \* 100

### cpc:

Cost per click.
Your average spend for one click.

CPC ($) = Spend / Clicks

### cpm:

Cost per mille.
Cost per one thousand ad serves.

CPM ($) = Spend / Impressions \* 1000

### cpa:

Cost per acquisition.
Your average spend per conversion.

CPA ($) = Spend / Conversions

### clickCPA:

Cost-per-click acquisition.
Your average spend for a conversion that happens after someone clicks your ad.

Click CPA ($) = Spend / Click Conversions

### viewCPA:

Cost-per-view acquisition: Your average spend for a
conversion that happens after someone views your ad.

View CPA ($) = Cost / View Throughs

### averageOrderValue:

Average Order Value
Average revenue per attributed conversion.

Average Order Value ($) = Attributed Revenue / Conversions

### ctcRate:

Click-through conversion rate.
The percentage of clicks that resulted in a click-through conversion.

CTC Rate (%) = Click Conversions / Clicks \* 100

### vtcRate:

View-through conversion rate: The percentage of impressions
that resulted in a view-through conversion.

VTC Rate (%) = View Throughs / Impressions \* 100

### roas:

Return on advertising spend: Your profit per dollar spent
on ads.

ROAS (x) = (Click Revenue + View Revenue) / Cost

### clickROAS:

Click return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone clicks
your ad.

Click ROAS (x) = Click Revenue / Cost

### viewROAS:

View return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone views
your ad.

View ROAS (x) = View Revenue / Cost

### roi:

Alias for ‘roas’.

### clickROI:

Alias for ‘clickROAS’.

### viewROI:

Alias for ‘viewROAS’.

### influencedThroughs:

Influenced Conversions.

A conversion touched or assisted by an ad but not attributed due
to the current attribution model.

### influencedRevenue:

Influenced Revenue.

Revenue touched or assisted by an ad but not attributed due to
the current attribution model.

### audienceSizeNew:

### audienceSizeTotal:

### newVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyNewVisitors instead.

The number of unique new visitors who came to your site after
viewing a prospecting ad.

### engagedVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyEngagedVisitors instead.

The number of unique new visitors who have viewed at least 3 pages
on your site after viewing a prospecting ad.

### bouncedVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL.

Visitors who have only viewed one page and left your site
after viewing a prospecting ad.

### nonBouncedVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL.

Visitors who have only viewed more than one page after
viewing a prospecting ad.

### newVisitorCost:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyNewVisitorCost instead.

The cost for each unique new visitor that came to your site after
viewing a prospecting ad.

New Visitor Cost = cost / newVisitors

### engagedVisitorCost:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyEngagedVisitorCost instead.

The cost for each unique new visitor that has viewed at least 3
pages on your site after viewing a prospecting ad

Engaged Visitor Cost = cost / engagedVisitors

### bounceRate:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL.

The percentage of new visitors who have only viewed one page
and left your site after viewing a prospecting ad.

Bounce Rate (%) = bouncedVisitors / newVisitors \* 100.

### dailyNewVisitors:

The number of daily new visitors who came to your site after
viewing a prospecting ad.

### dailyReturnVisitors:

The number of daily new visitors who return to your site after
viewing a prospecting ad.

### dailyEngagedVisitors:

The number of daily new visitors who have viewed at least 3 pages
on your site after viewing a prospecting ad.

### dailyBounceRate:

The percentage of daily new visitors who have only viewed one page
and left your site after viewing a prospecting ad.

### dailyNewVisitorCost:

The cost for each daily new visitor that came to your site after
viewing a prospecting ad.

New Visitor Cost = cost / dailyNewVisitors

### dailyEngagedVisitorCost:

The cost for each daily new visitor that has viewed at least 3
pages on your site after viewing a prospecting ad

Engaged Visitor Cost = cost / dailyEngagedVisitors

### sends:

Number of emails sent by a campaign.

### opens:

Number of unique-by-session email opens collected for a
campaign.

WARNING: this field is deprecated, please use “emailUniqueOpen” instead. To ease up
the transition this field will still be available, but always return null.

### openRate:

WARNING: this field is deprecated, please use “emailUniqueOpenRate”.
To ease up the transition this field will still be available, but always return null.

### emailScheduled: !

Total emails scheduled to be sent as part if this campaign.

### emailSentUnconfirmed: !

Total emails attempted to be sent.

### emailBounced: !

Deliveries that were rejected by the recipient's email service provider.

### emailSentConfirmed: !

Total emails confirmed to have been sent by the Email Service Provider.

### emailDeliveryRate: !

The percent of emails that have been confirmed to be delivered, over the send attempts.

### emailMarkedSpam: !

Recipients who report your emails as spam.

### emailUniqueMarkedSpam: !

Recipients who report your emails as spam, uniqued.

### emailUniqueOpen: !

When an email is opened by a user in its lifetime.

### emailUniqueOpenRate: !

The percent of sent emails that are opened once in a user's lifetime.

### emailUniqueClick: !

The number of times a link in an email was clicked once in a user's lifetime.

### emailUniqueClickRate: !

The percentage of emails opened that were clicked once in a user's lifetime.

### emailUniqueUnsubscribers: !

Recipients that unsubscribe from the email list, uniqued.

### emailUniqueUnsubscribeRate: !

The percent of recipients that have unsubscribers (unique) over the number of confirmed to be deliveries.

### emailUnsubscribers: !

Recipients that unsubscribe from the email list

### emailUniqueClicksByCountry:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times an email was clicked once in a user's lifetime broken out by ISO-2 country code

### emailUniqueOpensByCountry:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times an email is opened by a user in its lifetime, broken out by ISO-2 country code

### emailUniqueClicksByDeviceType:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times a link in an email was clicked once in a user's lifetime, broken out by device type
One of ‘pc’, ‘mobile’, ‘tablet’, ‘other’.

### emailUniqueOpensByDeviceType:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times an email is opened by a user in its lifetime, broken out by device type
One of ‘pc’, ‘mobile’, ‘tablet’, ‘other’.

### emailUniqueClicksByXpathUrl:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Unique clicks by xpath;url present in an email message
The key <xpath>;<url or macro> consists in 2 parts:
1. A XPath locator to the individual element that was clicked in the email message, based on a HTML5-compliant tree.
2. URL or macro: either a static URL that was clicked present in the email template or, the macro used to generate the URL. Eg.: {{product.url}}. Useful to identify links generated for the same intent, but it might show differently for emailed contacts.

In the future we may break this out to seperate metrics

### smsSentDelivered: !

Total number of SMS messages that were delivered (and confirmed by the recipient)

### smsClicks: !

Total number of times that a link in the SMS message was clicked.

### videoImpressions:

Impressions from video ads.

### videoViews:

Number of times the video begun playing.

### videoTwentyFivePercent:

Number of times at least 25% of the video duration was played.

### videoFiftyPercent:

Number of times at least 50% of the video duration was played.

### videoSeventyFivePercent:

Number of times at least 75% of the video duration was played.

### videoHundredPercent:

Number of times the full video duration was played.

### videoCompletionRate:

Video completion rate

Video Completion Rate (x) = Video Viewed To 100% / Video Impressions

### InventoryCampaign

**Fields**:

### eid: !

EID of the campaign.

### advertisable: !

EID of the advertisable to which this campaign belongs.

### budget: !

The daily budget of the campaign.
Note that this can be an approximation, for example when budgetType = “lifetime” it is:
budget = budgetGoal / numberOfDays(budgetStartDate, budgetEndDate)

### budgetGoal: !

The budget of the campaign, considered for the whole extent of its budgetType.
When budgetType = “lifetime”, it will be applied in the period since budgetStartDate until budgetEndDate.

### budgetType: !

The type of budget of the campaign (daily, lifetime…).
If this includes -auto (i.e. daily-auto), then it is the inventory campaign of a proxy strategy that is auto-balancing the budget for this campaign

### budgetStartDate:

The start date of a lifetime budget.

### budgetEndDate:

The end date of a lifetime budget.

### budgetSettingsString: !

Serialized budget settings as a string.
“budgetType,budgetStartDate,budgetEndDate,budgetGoal”

### createdDate:

The date this campaign was created.

### cpc: !

The CPC for this campaign.

### cpm: !

The CPM for this campaign.

### maxCpm: !

The maximum CPM for this campaign.

### name: !

The name of this campaign.

### startDate:

The day the campaign will start.

### endDate:

The day the campaign will end, exclusive.

### status: !

The status of the campaign.
One of ‘running’, ‘ended’, ‘paused’, ‘review’, ‘draft’, ‘rejected’ or ‘deleted’.
Result is ‘billingFailedPermanent’ or ‘billingFailedRecoverable’ when BillingAuthStatus is ‘failed’.

### actualStatus:

The effective status of the campaign.
Details the reasons why it is not running, if applicable.

### actualStatusString: !

Minimal string representation of the actual status.
One of ‘running’, ‘notRunning’ ,’ended’, ‘paused’, ‘review’, ‘draft’, ‘rejected’ or ‘deleted’.

### updatedDate:

The date this campaign was last updated.

### channel: !

Campaign channel: one of ‘email’, ‘social’ or ‘web’

### isConnectedChannel: !

True if the campaign is run by a third party.

### source: !

The service responsible for the creation of this campaign.

### currency: !

ISO-4217 currency code for the given amount.

### type: !

Type for the campaign. One of “prospecting”, “blended”r
“retargeting”.

### abmType: !

Type of ABM campaign.
Empty string if this is not an ABM campaign.

### targetingType: !

The type of targeting that is used to pick which customers will be reached by this campaign.

### kpiGoal: !

Goal -for the kpiMetric- that drives the campaign’s bid strategy.
Null for automatic.

### kpiCurrency: !

ISO 4217 currency code for kpiGoal.
If not provided assume the currency provided at the Advertisable level.

### kpiMetric: !

Metric being targeted by the campaign’s bid strategy.

### spendLimitUntil:

SpendLimitUntil

### spendLimitUntilReason: !

SpendLimitUntilReason

### processingStatus: !

The processing status of the campaign inside the AdRoll.
It may have a transient value other than “created” while
the campaign is being processed by an internal job.

### billingAuthStatus:

The billing auth status of the campaign inside the AdRoll.
Will default to empty string when API BillingAuthStatus not present.
Result is “failed” when the billing authorization did not complete.

### playbookEID: !

The parent Playbook’s EID for the campaign, only if it exists.

### playbookName: !

The parent Playbook’s Name for the campaign, only if it exists.

### playbookType: !

The parent Playbook’s Type for the campaign, only if it exists.

### inVoltronStrategyEID: !

The EID of this campaign as referenced from its Voltron strategy.
Only available for inventory campaigns of Universal Campaigns.

### proxyStrategyEID: !

The eid of the Proxy Strategy that contains this campaign. Only for Inventory campaigns.

### proxyStrategyIsFrozen: !

The isFrozen value of the Proxy Strategy that contains this campaign. Only for Inventory campaigns.

### proxyStrategyStatus: !

The status of the Proxy Strategy that contains this campaign. Only for Inventory campaigns.

### proxyStrategyName: !

The name of the Proxy Strategy that contains this campaign. Only for Inventory campaigns.

### newsletterScheduled: !

If this is an Email Newsletter campaign, the number of potential recipients.

### newsletterSends: !

If this is an Email Newsletter campaign, the number of emails sent.

### newsletterScheduledDate:

If this is an Email Newsletter campaign, the scheduled date for delivery.
Only if the delivery is scheduled to happen or of it has already occurred. Omitted if in draft, paused or cancelled.

### isBillable: !

True if the campaign is run by NextRoll and will be directly billed to
the advertisable’s account. False if it is run by a third party.

### isFrozen: !

True if the strategy is frozen, and no changes can be made to it.

### syncStatus: !

Only for Connected Campaigns, indicates the status of the sync’ing with the external service.
When available, can be one of “pending”, “synced” or “error”

### syncError: !

Only for Connected Campaigns, shows the error that caused the sync’ing with the external service to fail.
Provided if the syncStatus field is “error”.

### facebookAdsManagerPermalink: !

DEPRECATED: please use adsManagerPermalink instead

### adsManagerPermalink: !

The URL to the campaign if it has been externally connected.

### isIntegrated: !

### useCase: !

### objective: !

The campaign marketing objective returned by AdRoll API.

### funnelStage:

Funnel stage for the campaign. One of “awareness”, “consideration”, “conversion”, or “other”.

### isBudgetBalancingAutomated: !

Indicates if this campaign is a strategy that balances the budget automatically across its inventory campaigns.
False means that inventory campaign budgets are manually set.

### possibleStatusChanges: [!]

Available status changes for the current campaign. BETA.

### performanceTargets: []

PerformanceTargets

### tags: [!]

Internal tags set on creation.

### automationEID:

If managed by an Automation, the EID of the Automation.

### automationNodeEID:

If managed by an Automation,
the EID of the Automation Node that references this entity.

### automationName:

If managed by an Automation, the name of the Automation.

### disabled: !

Indicates if the campaign is disabled.
Currently applies only to Automation-managed campaigns that have been disabled by subscription downgrade action.

### klaviyoFlowEID:

If managed by a Klaviyo Flow, the EID of the Flow.

### klaviyoFlowName:

If managed by a Klaviyo Flow, the name of the Flow.

### campaignGroupEID: !

EID for the parent Universal/Proxy campaign group.

### campaignGroupName: !

Name for the parent Universal/Proxy campaign group.

### adgroups: []!

Adgroups for this Campaign.

### emails: []!

Emails for this Campaign

### audiences(includeInactive:) : []!

Audiences for this Campaign.

**Arguments**:

### includeInactive:

True to return also inactive audiences (those that have been deleted).
By default only active audiences are included.

* **Default:**
  false

### metrics(start: , end: , pastDays: , currency: , duration:) : !

Metrics for the Campaign.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The
date range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The
date range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### duration:

[DEPRECATED] Unused.

* **Default:**
  30

### conversions(start: , end: , pastDays: , currency:) : !

Metrics for the entity broken down by conversion audiences.

**Arguments**:

### start:

The start date for the metrics period (inclusive). The date
range will be: [start, end)

### end:

The end date for the metrics period (exclusive). The date
range will be: [start, end)

### pastDays:

Alternative to start/end parameters with less precedence.
The date range will be: [today_utc - pastDays, today_utc)

* **Default:**
  0

### currency:

Currency to load the metrics in.

* **Default:**
  “USD”

### Keyword

Contains reporting metric data by keyword for Google Search campaign-adgroups.

**Fields**:

### keyword: !

Keyword in the Google Search adgroup…

### impressions: !

The sum of the number of ad impressions.

### clicks: !

The sum of clicks of all kinds of ads and emails.

### cost: !

Cost associated to all kinds of ads and emails.

### conversions: !

Conversions
Total.
Conversions (count) = View Conversions + Click Conversions

### clickThroughs: !

Click-through conversion (CTC).
A goal completion that happens after someone clicks your ad.

### viewThroughs: !

View-through conversion (VTC).
A goal completion that happens after someone views your ad, but
does not click.

### revenue: !

Revenue (amount) = View Revenue + Click Conversions

### clickRevenue: !

Click-Attributed Revenue.
Total earnings when someone clicks your ad and converts.

### viewRevenue: !

View-Attributed Revenue.
Total earnings when someone views your ad and converts.

### ctr: !

Click-through rate.
The percentage of ad serves that were clicked.

CTR (%) = Clicks / Impression \* 100

### cpc: !

Cost per click.
Your average spend for one click.

CPC ($) = Spend / Clicks

### cpm: !

Cost per mille.
Cost per one thousand ad serves.

CPM ($) = Spend / Impressions \* 1000

### cpa: !

Cost per acquisition.
Your average spend per conversion.

CPA ($) = Spend / Conversions

### clickCPA: !

Cost-per-click acquisition.
Your average spend for a conversion that happens after someone clicks your ad.

Click CPA ($) = Spend / Click Conversions

### viewCPA: !

Cost-per-view acquisition: Your average spend for a
conversion that happens after someone views your ad.

View CPA ($) = Cost / View Throughs

### averageOrderValue: !

Average Order Value
Average revenue per attributed conversion.

Average Order Value ($) = Attributed Revenue / Conversions

### ctcRate: !

Click-through conversion rate.
The percentage of clicks that resulted in a click-through conversion.

CTC Rate (%) = Click Conversions / Clicks \* 100

### vtcRate: !

View-through conversion rate: The percentage of impressions
that resulted in a view-through conversion.

VTC Rate (%) = View Throughs / Impressions \* 100

### roas: !

Return on advertising spend: Your profit per dollar spent
on ads.

ROAS (x) = (Click Revenue + View Revenue) / Cost

### clickROAS: !

Click return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone clicks
your ad.

Click ROAS (x) = Click Revenue / Cost

### viewROAS: !

View return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone views
your ad.

View ROAS (x) = View Revenue / Cost

### KeywordResult

**Fields**:

### byKeyword: [!]!

Summarizes by Google Search keyword the reporting data for the given date range.
[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Currently Fetching Keywords and keyword metrics without also
requesting metrics for parent adgroup or campaign will return empty result.

### LogEvent

Represents a single log event.

**Fields**:

### info: !

Provides the formatted summary line for the timeline item.

This includes information from level, name, message, and delta.

### level: !

Level for this log event.

### name: !

Log name for the entry.

### message: !

Message for the log entry.

### delta: !

Time in seconds for this entry, relative to the start of the request.

### time: !

Time for this entry in RFC3339 format.

### fields:

Additional fields associated with the log entry.

### caller: !

Caller for this entry.

### stack: [!]!

Stack trace for this entry.

### kind: !

Alias to fields.kind.

### operation: !

Alias to fields.operation.

### operationRequest: !

Combined field to describe internal requests.
“METHOD URL”

### key: !

Returns a key that relates to the log entry code and target operation.

This combines the log name with the request root and numeric IDs stripped,
with the operation when available.

### LogItem

[WARNING] Log lines are intended for internal analysis and debugging.

They are not available for external developers to consume.

Represents a single entry in the operation log for the query.

**Fields**:

### info: !

The kind, key, text and timing information for the entry in a single field, for convenience.

### kind: !

Kind of operation referred by this log entry.

### key: !

Key for the operation that generated this log entry.

### text: !

Text for the log entry.

### start:

Start time for the operation in the log entry.

### end:

End time for the operation in the log entry.

### delta: !

Delta in seconds for the operation start from the query start.

### duration: !

Duration in seconds for the operation.

### lines(filter:) : [!]!

The log entry text and/or data split by lines.

**Arguments**:

### filter:

Empty to return the log entry text and default data (i.e.
unnamed data).

If provided, will return lines for the given data filter. In
that case, this is a shortcut to querying:

> data(filter:”some filter”) { lines }
* **Default:**
  null

### data(filter:) :

Additional data for the log entry.

**Arguments**:

### filter:

Filter the returned data by name. If this is empty, only the
default (i.e. unnamed) data will be returned.

This supports wildcard \* characters to match anything. If
the wildcard follows a dot (i.e. .\*) the dot is made
optional (e.g. name.\* will match both name and name.child).

* **Default:**
  null

### json(filter:) :

Additional data for the log entry as JSON.

This is a shortcut for querying:

> data(filter:”some filter”) { json }

This is null if the given data cannot be converted to JSON.

**Arguments**:

### filter:

This is the filter to apply for the data (see data field
for details).

* **Default:**
  null

### allData: [!]!

Return all data items for the entry.

### LogItemData

[WARNING] Log lines are intended for internal analysis and debugging.

They are not available for external developers to consume.

Data entry for a LogItem.

**Fields**:

### name: !

Name for this entry. This can be used with LogItem.data
and LogData.lines.

### text: !

Raw data for the entry.

### lines: [!]

Text for the entry split by lines.

### json:

Text for the entry converted to a JSON value, or null if cannot
be converted.

### LogRoot

**Fields**:

### events: [!]!

Log events.

### Metric

Contains reporting metric data for attributions, deliveries,

segment deliveries and emails.

**Fields**:

### date:

Date for this particular metric data. This is empty for
summaries.

### impressions:

The sum of the number of ad impressions.

### clicks:

The sum of clicks of all kinds of ads and emails.

### cost:

Cost associated to all kinds of ads and emails.

### conversions:

Conversions
Total.
Conversions (count) = View Conversions + Click Conversions

### clickThroughs:

Click-through conversion (CTC).
A goal completion that happens after someone clicks your ad.

To get the noise from ARA click-throughs, take the square root of araClickThroughsVariance.

### viewThroughs:

View-through conversion (VTC).
A goal completion that happens after someone views your ad, but
does not click.

To get the noise from ARA view-throughs, take the square root of araViewThroughsVariance.

### revenue:

Revenue (amount) = View Revenue + Click Conversions

### clickRevenue:

Click-Attributed Revenue.
Total earnings when someone clicks your ad and converts.

To get the noise from ARA click-throughs, subtract araClickRevenueMin from araClickRevenueMax.

### viewRevenue:

View-Attributed Revenue.
Total earnings when someone views your ad and converts.

To get the noise from ARA view-throughs, subtract araViewRevenueMin from araViewRevenueMax.

### ctr:

Click-through rate.
The percentage of ad serves that were clicked.

CTR (%) = Clicks / Impression \* 100

### cpc:

Cost per click.
Your average spend for one click.

CPC ($) = Spend / Clicks

### cpm:

Cost per mille.
Cost per one thousand ad serves.

CPM ($) = Spend / Impressions \* 1000

### cpa:

Cost per acquisition.
Your average spend per conversion.

CPA ($) = Spend / Conversions

### clickCPA:

Cost-per-click acquisition.
Your average spend for a conversion that happens after someone clicks your ad.

Click CPA ($) = Spend / Click Conversions

### viewCPA:

Cost-per-view acquisition: Your average spend for a
conversion that happens after someone views your ad.

View CPA ($) = Cost / View Throughs

### averageOrderValue:

Average Order Value
Average revenue per attributed conversion.

Average Order Value ($) = Attributed Revenue / Conversions

### ctcRate:

Click-through conversion rate.
The percentage of clicks that resulted in a click-through conversion.

CTC Rate (%) = Click Conversions / Clicks \* 100

### vtcRate:

View-through conversion rate: The percentage of impressions
that resulted in a view-through conversion.

VTC Rate (%) = View Throughs / Impressions \* 100

### roas:

Return on advertising spend: Your profit per dollar spent
on ads.

ROAS (x) = (Click Revenue + View Revenue) / Cost

### clickROAS:

Click return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone clicks
your ad.

Click ROAS (x) = Click Revenue / Cost

### viewROAS:

View return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone views
your ad.

View ROAS (x) = View Revenue / Cost

### roi:

Alias for ‘roas’.

### clickROI:

Alias for ‘clickROAS’.

### viewROI:

Alias for ‘viewROAS’.

### influencedThroughs:

Influenced Conversions.

A conversion touched or assisted by an ad but not attributed due
to the current attribution model.

### influencedRevenue:

Influenced Revenue.

Revenue touched or assisted by an ad but not attributed due to
the current attribution model.

### audienceSizeNew:

### audienceSizeTotal:

### newVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyNewVisitors instead.

The number of unique new visitors who came to your site after
viewing a prospecting ad.

### engagedVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyEngagedVisitors instead.

The number of unique new visitors who have viewed at least 3 pages
on your site after viewing a prospecting ad.

### bouncedVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL.

Visitors who have only viewed one page and left your site
after viewing a prospecting ad.

### nonBouncedVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL.

Visitors who have only viewed more than one page after
viewing a prospecting ad.

### newVisitorCost:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyNewVisitorCost instead.

The cost for each unique new visitor that came to your site after
viewing a prospecting ad.

New Visitor Cost = cost / newVisitors

### engagedVisitorCost:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyEngagedVisitorCost instead.

The cost for each unique new visitor that has viewed at least 3
pages on your site after viewing a prospecting ad

Engaged Visitor Cost = cost / engagedVisitors

### bounceRate:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL.

The percentage of new visitors who have only viewed one page
and left your site after viewing a prospecting ad.

Bounce Rate (%) = bouncedVisitors / newVisitors \* 100.

### dailyNewVisitors:

The number of daily new visitors who came to your site after
viewing a prospecting ad.

### dailyReturnVisitors:

The number of daily new visitors who return to your site after
viewing a prospecting ad.

### dailyEngagedVisitors:

The number of daily new visitors who have viewed at least 3 pages
on your site after viewing a prospecting ad.

### dailyBounceRate:

The percentage of daily new visitors who have only viewed one page
and left your site after viewing a prospecting ad.

### dailyNewVisitorCost:

The cost for each daily new visitor that came to your site after
viewing a prospecting ad.

New Visitor Cost = cost / dailyNewVisitors

### dailyEngagedVisitorCost:

The cost for each daily new visitor that has viewed at least 3
pages on your site after viewing a prospecting ad

Engaged Visitor Cost = cost / dailyEngagedVisitors

### sends:

Number of emails sent by a campaign.

### opens:

Number of unique-by-session email opens collected for a
campaign.

WARNING: this field is deprecated, please use “emailUniqueOpen” instead. To ease up
the transition this field will still be available, but always return null.

### openRate:

WARNING: this field is deprecated, please use “emailUniqueOpenRate”.
To ease up the transition this field will still be available, but always return null.

### emailScheduled: !

Total emails scheduled to be sent as part if this campaign.

### emailSentUnconfirmed: !

Total emails attempted to be sent.

### emailBounced: !

Deliveries that were rejected by the recipient's email service provider.

### emailSentConfirmed: !

Total emails confirmed to have been sent by the Email Service Provider.

### emailDeliveryRate: !

The percent of emails that have been confirmed to be delivered, over the send attempts.

### emailMarkedSpam: !

Recipients who report your emails as spam.

### emailUniqueMarkedSpam: !

Recipients who report your emails as spam, uniqued.

### emailUniqueOpen: !

When an email is opened by a user in its lifetime.

### emailUniqueOpenRate: !

The percent of sent emails that are opened once in a user's lifetime.

### emailUniqueClick: !

The number of times a link in an email was clicked once in a user's lifetime.

### emailUniqueClickRate: !

The percentage of emails opened that were clicked once in a user's lifetime.

### emailUniqueUnsubscribers: !

Recipients that unsubscribe from the email list, uniqued.

### emailUniqueUnsubscribeRate: !

The percent of recipients that have unsubscribers (unique) over the number of confirmed to be deliveries.

### emailUnsubscribers: !

Recipients that unsubscribe from the email list

### emailUniqueClicksByCountry:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times an email was clicked once in a user's lifetime broken out by ISO-2 country code

### emailUniqueOpensByCountry:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times an email is opened by a user in its lifetime, broken out by ISO-2 country code

### emailUniqueClicksByDeviceType:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times a link in an email was clicked once in a user's lifetime, broken out by device type
One of ‘pc’, ‘mobile’, ‘tablet’, ‘other’.

### emailUniqueOpensByDeviceType:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times an email is opened by a user in its lifetime, broken out by device type
One of ‘pc’, ‘mobile’, ‘tablet’, ‘other’.

### emailUniqueClicksByXpathUrl:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Unique clicks by xpath;url present in an email message
The key <xpath>;<url or macro> consists in 2 parts:
1. A XPath locator to the individual element that was clicked in the email message, based on a HTML5-compliant tree.
2. URL or macro: either a static URL that was clicked present in the email template or, the macro used to generate the URL. Eg.: {{product.url}}. Useful to identify links generated for the same intent, but it might show differently for emailed contacts.

In the future we may break this out to seperate metrics

### smsSentDelivered: !

Total number of SMS messages that were delivered (and confirmed by the recipient)

### smsClicks: !

Total number of times that a link in the SMS message was clicked.

### videoImpressions:

Impressions from video ads.

### videoViews:

Number of times the video begun playing.

### videoTwentyFivePercent:

Number of times at least 25% of the video duration was played.

### videoFiftyPercent:

Number of times at least 50% of the video duration was played.

### videoSeventyFivePercent:

Number of times at least 75% of the video duration was played.

### videoHundredPercent:

Number of times the full video duration was played.

### videoCompletionRate:

Video completion rate

Video Completion Rate (x) = Video Viewed To 100% / Video Impressions

### frequency: !

Number of ads seen per day by reached users (only applies to WEB campaigns)

Frequency = total impressions/reached users

### deviceFrequency: !

Number of ads seen per day by reached devices (only applies to CTV campaigns)

Device Frequency = total impressions/reached devices

### totalUniqueHHsReached:

Number of distinct households that received CTV impressions on a given day

### uniqueHHSiteVisits:

Number of distinct households that visited the site, after viewing an ad

### customMetric(formula:) : !

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Usage:
- Operators: ‘+’, ‘-’, ‘\*’, ‘/’ and parentheses () are valid
Requires formula to have space-seperated operand and operators.

e.g. costPerImpression: customMetric(formula: “cost / impressions”)

**Arguments**:

### formula:

### MetricAggregateResult

Groups reporting metric data in summary and by date format. This

is the result of the metricsTotal field. See the root metricsTotal

field in Query for documentation.

**Fields**:

### summary: !

Summarizes the reporting data for the given date range.

### byDate: [!]!

Reporting data by date in the given range.

### MetricCountry

Contains reporting metric data for country

**Fields**:

### date:

Date for this particular metric data. This is empty for
summaries.

### impressions:

The sum of the number of ad impressions.

### clicks:

The sum of clicks of all kinds of ads and emails.

### cost:

Cost associated to all kinds of ads and emails.

### conversions:

Conversions Total.
Conversions (count) = View Conversions + Click Conversions

### MetricCountryResult

Groups reporting metric data for the country in summary and by

date format.

**Fields**:

### country: !

The country this metric pertains to.

### countryCode: !

ISO-2 country code

### summary: !

Summarizes the reporting data for the given date range.

### byDate: [!]!

Reporting data by date in the given range.

### MetricDomain

Contains reporting metric data for the domain.

**Fields**:

### date:

Date for this particular metric data. This is empty for
summaries.

### impressions: !

The sum of the number of ad impressions on the domain.

### clicks: !

The sum of clicks of ads on the domain.

### cost: !

Cost associated to displaying ads on the domain.

### cpm: !

Cost per mille.
Cost per one thousand ad serves on the domain.

CPM ($) = Spend / Impressions \* 1000

### ctr: !

Click-through rate.
The percentage of ad serves that were clicked on the domain.

CTR (%) = Clicks / Impression \* 100

### MetricDomainResult

Groups reporting metric data for the domain in summary and by

date format.

**Fields**:

### domain: !

The domain this metric pertains to.

### summary: !

Summarizes the reporting data for the given date range.

### byDate: [!]!

Reporting data by date in the given range.

### MetricForAdvertisable

Contains advertisable level reporting metric data for attributions, deliveries,

segment deliveries and emails.

**Fields**:

### date:

Date for this particular metric data. This is empty for
summaries.

### impressions:

The sum of the number of ad impressions.

### clicks:

The sum of clicks of all kinds of ads and emails.

### cost:

Cost associated to all kinds of ads and emails.

### conversions:

Conversions
Total.
Conversions (count) = View Conversions + Click Conversions

### clickThroughs:

Click-through conversion (CTC).
A goal completion that happens after someone clicks your ad.

To get the noise from ARA click-throughs, take the square root of araClickThroughsVariance.

### viewThroughs:

View-through conversion (VTC).
A goal completion that happens after someone views your ad, but
does not click.

To get the noise from ARA view-throughs, take the square root of araViewThroughsVariance.

### revenue:

Revenue (amount) = View Revenue + Click Conversions

### clickRevenue:

Click-Attributed Revenue.
Total earnings when someone clicks your ad and converts.

To get the noise from ARA click-throughs, subtract araClickRevenueMin from araClickRevenueMax.

### viewRevenue:

View-Attributed Revenue.
Total earnings when someone views your ad and converts.

To get the noise from ARA view-throughs, subtract araViewRevenueMin from araViewRevenueMax.

### ctr:

Click-through rate.
The percentage of ad serves that were clicked.

CTR (%) = Clicks / Impression \* 100

### cpc:

Cost per click.
Your average spend for one click.

CPC ($) = Spend / Clicks

### cpm:

Cost per mille.
Cost per one thousand ad serves.

CPM ($) = Spend / Impressions \* 1000

### cpa:

Cost per acquisition.
Your average spend per conversion.

CPA ($) = Spend / Conversions

### clickCPA:

Cost-per-click acquisition.
Your average spend for a conversion that happens after someone clicks your ad.

Click CPA ($) = Spend / Click Conversions

### viewCPA:

Cost-per-view acquisition: Your average spend for a
conversion that happens after someone views your ad.

View CPA ($) = Cost / View Throughs

### averageOrderValue:

Average Order Value
Average revenue per attributed conversion.

Average Order Value ($) = Attributed Revenue / Conversions

### ctcRate:

Click-through conversion rate.
The percentage of clicks that resulted in a click-through conversion.

CTC Rate (%) = Click Conversions / Clicks \* 100

### vtcRate:

View-through conversion rate: The percentage of impressions
that resulted in a view-through conversion.

VTC Rate (%) = View Throughs / Impressions \* 100

### roas:

Return on advertising spend: Your profit per dollar spent
on ads.

ROAS (x) = (Click Revenue + View Revenue) / Cost

### clickROAS:

Click return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone clicks
your ad.

Click ROAS (x) = Click Revenue / Cost

### viewROAS:

View return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone views
your ad.

View ROAS (x) = View Revenue / Cost

### roi:

Alias for ‘roas’.

### clickROI:

Alias for ‘clickROAS’.

### viewROI:

Alias for ‘viewROAS’.

### influencedThroughs:

Influenced Conversions.

A conversion touched or assisted by an ad but not attributed due
to the current attribution model.

### influencedRevenue:

Influenced Revenue.

Revenue touched or assisted by an ad but not attributed due to
the current attribution model.

### audienceSizeNew:

### audienceSizeTotal:

### newVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyNewVisitors instead.

The number of unique new visitors who came to your site after
viewing a prospecting ad.

### engagedVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyEngagedVisitors instead.

The number of unique new visitors who have viewed at least 3 pages
on your site after viewing a prospecting ad.

### bouncedVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL.

Visitors who have only viewed one page and left your site
after viewing a prospecting ad.

### nonBouncedVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL.

Visitors who have only viewed more than one page after
viewing a prospecting ad.

### newVisitorCost:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyNewVisitorCost instead.

The cost for each unique new visitor that came to your site after
viewing a prospecting ad.

New Visitor Cost = cost / newVisitors

### engagedVisitorCost:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyEngagedVisitorCost instead.

The cost for each unique new visitor that has viewed at least 3
pages on your site after viewing a prospecting ad

Engaged Visitor Cost = cost / engagedVisitors

### bounceRate:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL.

The percentage of new visitors who have only viewed one page
and left your site after viewing a prospecting ad.

Bounce Rate (%) = bouncedVisitors / newVisitors \* 100.

### dailyNewVisitors:

The number of daily new visitors who came to your site after
viewing a prospecting ad.

### dailyReturnVisitors:

The number of daily new visitors who return to your site after
viewing a prospecting ad.

### dailyEngagedVisitors:

The number of daily new visitors who have viewed at least 3 pages
on your site after viewing a prospecting ad.

### dailyBounceRate:

The percentage of daily new visitors who have only viewed one page
and left your site after viewing a prospecting ad.

### dailyNewVisitorCost:

The cost for each daily new visitor that came to your site after
viewing a prospecting ad.

New Visitor Cost = cost / dailyNewVisitors

### dailyEngagedVisitorCost:

The cost for each daily new visitor that has viewed at least 3
pages on your site after viewing a prospecting ad

Engaged Visitor Cost = cost / dailyEngagedVisitors

### sends:

Number of emails sent by a campaign.

### opens:

Number of unique-by-session email opens collected for a
campaign.

WARNING: this field is deprecated, please use “emailUniqueOpen” instead. To ease up
the transition this field will still be available, but always return null.

### openRate:

WARNING: this field is deprecated, please use “emailUniqueOpenRate”.
To ease up the transition this field will still be available, but always return null.

### emailScheduled: !

Total emails scheduled to be sent as part if this campaign.

### emailSentUnconfirmed: !

Total emails attempted to be sent.

### emailBounced: !

Deliveries that were rejected by the recipient's email service provider.

### emailSentConfirmed: !

Total emails confirmed to have been sent by the Email Service Provider.

### emailDeliveryRate: !

The percent of emails that have been confirmed to be delivered, over the send attempts.

### emailMarkedSpam: !

Recipients who report your emails as spam.

### emailUniqueMarkedSpam: !

Recipients who report your emails as spam, uniqued.

### emailUniqueOpen: !

When an email is opened by a user in its lifetime.

### emailUniqueOpenRate: !

The percent of sent emails that are opened once in a user's lifetime.

### emailUniqueClick: !

The number of times a link in an email was clicked once in a user's lifetime.

### emailUniqueClickRate: !

The percentage of emails opened that were clicked once in a user's lifetime.

### emailUniqueUnsubscribers: !

Recipients that unsubscribe from the email list, uniqued.

### emailUniqueUnsubscribeRate: !

The percent of recipients that have unsubscribers (unique) over the number of confirmed to be deliveries.

### emailUnsubscribers: !

Recipients that unsubscribe from the email list

### emailUniqueClicksByCountry:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times an email was clicked once in a user's lifetime broken out by ISO-2 country code

### emailUniqueOpensByCountry:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times an email is opened by a user in its lifetime, broken out by ISO-2 country code

### emailUniqueClicksByDeviceType:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times a link in an email was clicked once in a user's lifetime, broken out by device type
One of ‘pc’, ‘mobile’, ‘tablet’, ‘other’.

### emailUniqueOpensByDeviceType:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times an email is opened by a user in its lifetime, broken out by device type
One of ‘pc’, ‘mobile’, ‘tablet’, ‘other’.

### emailUniqueClicksByXpathUrl:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Unique clicks by xpath;url present in an email message
The key <xpath>;<url or macro> consists in 2 parts:
1. A XPath locator to the individual element that was clicked in the email message, based on a HTML5-compliant tree.
2. URL or macro: either a static URL that was clicked present in the email template or, the macro used to generate the URL. Eg.: {{product.url}}. Useful to identify links generated for the same intent, but it might show differently for emailed contacts.

In the future we may break this out to seperate metrics

### smsSentDelivered: !

Total number of SMS messages that were delivered (and confirmed by the recipient)

### smsClicks: !

Total number of times that a link in the SMS message was clicked.

### videoImpressions:

Impressions from video ads.

### videoViews:

Number of times the video begun playing.

### videoTwentyFivePercent:

Number of times at least 25% of the video duration was played.

### videoFiftyPercent:

Number of times at least 50% of the video duration was played.

### videoSeventyFivePercent:

Number of times at least 75% of the video duration was played.

### videoHundredPercent:

Number of times the full video duration was played.

### videoCompletionRate:

Video completion rate

Video Completion Rate (x) = Video Viewed To 100% / Video Impressions

### frequency: !

Number of ads seen per day by reached users (only applies to WEB campaigns)

Frequency = total impressions/reached users

### deviceFrequency: !

Number of ads seen per day by reached devices (only applies to CTV campaigns)

Device Frequency = total impressions/reached devices

### totalUniqueHHsReached:

Number of distinct households that received CTV impressions on a given day

### uniqueHHSiteVisits:

Number of distinct households that visited the site, after viewing an ad

### siteBounceRate:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteNewVisitors:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteNewVisitorsNot:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteEngaged:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteEngagedNot:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteEngagedNewVisitors:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteEngagedNewVisitorsNot:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteAddToCart:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteAddToCartNot:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteConverters:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteConvertersNot:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteReturningVisitors:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteReturningVisitorsNot:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### convCountImpRate01: !

Number of converters who saw an average of 0-1 ads/day in the last 30 days.

### convCountImpRate12: !

Number of converters who saw an average of 1-2 ads/day in the last 30 days.

### convCountImpRate23: !

Number of converters who saw an average of 2-3 ads/day in the last 30 days.

### convCountImpRate34: !

Number of converters who saw an average of 3-4 ads/day in the last 30 days.

### convCountImpRate4: !

Number of converters who saw an average of 4+ ads/day in the last 30 days.

### nonConvCountImpRate01: !

Number of non-converters who saw an average of 0-1 ads/day in the last 30 days.

### nonConvCountImpRate12: !

Number of non-converters who saw an average of 1-2 ads/day in the last 30 days.

### nonConvCountImpRate23: !

Number of non-converters who saw an average of 2-3 ads/day in the last 30 days.

### nonConvCountImpRate34: !

Number of non-converters who saw an average of 3-4 ads/day in the last 30 days.

### nonConvCountImpRate4: !

Number of non-converters who saw an average of 4+ ads/day in the last 30 days.

### customMetric(formula:) : !

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Usage:
- Operators: ‘+’, ‘-’, ‘\*’, ‘/’ and parentheses () are valid
Requires formula to have space-seperated operand and operators.

e.g. costPerImpression: customMetric(formula: “cost / impressions”)

**Arguments**:

### formula:

### MetricForCampaign

Contains campaign level reporting metric data for attributions, deliveries,

segment deliveries and emails.

**Fields**:

### date:

Date for this particular metric data. This is empty for
summaries.

### impressions:

The sum of the number of ad impressions.

### clicks:

The sum of clicks of all kinds of ads and emails.

### cost:

Cost associated to all kinds of ads and emails.

### conversions:

Conversions
Total.
Conversions (count) = View Conversions + Click Conversions

### clickThroughs:

Click-through conversion (CTC).
A goal completion that happens after someone clicks your ad.

To get the noise from ARA click-throughs, take the square root of araClickThroughsVariance.

### viewThroughs:

View-through conversion (VTC).
A goal completion that happens after someone views your ad, but
does not click.

To get the noise from ARA view-throughs, take the square root of araViewThroughsVariance.

### revenue:

Revenue (amount) = View Revenue + Click Conversions

### clickRevenue:

Click-Attributed Revenue.
Total earnings when someone clicks your ad and converts.

To get the noise from ARA click-throughs, subtract araClickRevenueMin from araClickRevenueMax.

### viewRevenue:

View-Attributed Revenue.
Total earnings when someone views your ad and converts.

To get the noise from ARA view-throughs, subtract araViewRevenueMin from araViewRevenueMax.

### ctr:

Click-through rate.
The percentage of ad serves that were clicked.

CTR (%) = Clicks / Impression \* 100

### cpc:

Cost per click.
Your average spend for one click.

CPC ($) = Spend / Clicks

### cpm:

Cost per mille.
Cost per one thousand ad serves.

CPM ($) = Spend / Impressions \* 1000

### cpa:

Cost per acquisition.
Your average spend per conversion.

CPA ($) = Spend / Conversions

### clickCPA:

Cost-per-click acquisition.
Your average spend for a conversion that happens after someone clicks your ad.

Click CPA ($) = Spend / Click Conversions

### viewCPA:

Cost-per-view acquisition: Your average spend for a
conversion that happens after someone views your ad.

View CPA ($) = Cost / View Throughs

### averageOrderValue:

Average Order Value
Average revenue per attributed conversion.

Average Order Value ($) = Attributed Revenue / Conversions

### ctcRate:

Click-through conversion rate.
The percentage of clicks that resulted in a click-through conversion.

CTC Rate (%) = Click Conversions / Clicks \* 100

### vtcRate:

View-through conversion rate: The percentage of impressions
that resulted in a view-through conversion.

VTC Rate (%) = View Throughs / Impressions \* 100

### roas:

Return on advertising spend: Your profit per dollar spent
on ads.

ROAS (x) = (Click Revenue + View Revenue) / Cost

### clickROAS:

Click return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone clicks
your ad.

Click ROAS (x) = Click Revenue / Cost

### viewROAS:

View return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone views
your ad.

View ROAS (x) = View Revenue / Cost

### roi:

Alias for ‘roas’.

### clickROI:

Alias for ‘clickROAS’.

### viewROI:

Alias for ‘viewROAS’.

### influencedThroughs:

Influenced Conversions.

A conversion touched or assisted by an ad but not attributed due
to the current attribution model.

### influencedRevenue:

Influenced Revenue.

Revenue touched or assisted by an ad but not attributed due to
the current attribution model.

### audienceSizeNew:

### audienceSizeTotal:

### newVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyNewVisitors instead.

The number of unique new visitors who came to your site after
viewing a prospecting ad.

### engagedVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyEngagedVisitors instead.

The number of unique new visitors who have viewed at least 3 pages
on your site after viewing a prospecting ad.

### bouncedVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL.

Visitors who have only viewed one page and left your site
after viewing a prospecting ad.

### nonBouncedVisitors:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL.

Visitors who have only viewed more than one page after
viewing a prospecting ad.

### newVisitorCost:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyNewVisitorCost instead.

The cost for each unique new visitor that came to your site after
viewing a prospecting ad.

New Visitor Cost = cost / newVisitors

### engagedVisitorCost:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL. Use dailyEngagedVisitorCost instead.

The cost for each unique new visitor that has viewed at least 3
pages on your site after viewing a prospecting ad

Engaged Visitor Cost = cost / engagedVisitors

### bounceRate:

This field has been deprecated as metrics for it are no longer available
and it will always be NULL.

The percentage of new visitors who have only viewed one page
and left your site after viewing a prospecting ad.

Bounce Rate (%) = bouncedVisitors / newVisitors \* 100.

### dailyNewVisitors:

The number of daily new visitors who came to your site after
viewing a prospecting ad.

### dailyReturnVisitors:

The number of daily new visitors who return to your site after
viewing a prospecting ad.

### dailyEngagedVisitors:

The number of daily new visitors who have viewed at least 3 pages
on your site after viewing a prospecting ad.

### dailyBounceRate:

The percentage of daily new visitors who have only viewed one page
and left your site after viewing a prospecting ad.

### dailyNewVisitorCost:

The cost for each daily new visitor that came to your site after
viewing a prospecting ad.

New Visitor Cost = cost / dailyNewVisitors

### dailyEngagedVisitorCost:

The cost for each daily new visitor that has viewed at least 3
pages on your site after viewing a prospecting ad

Engaged Visitor Cost = cost / dailyEngagedVisitors

### sends:

Number of emails sent by a campaign.

### opens:

Number of unique-by-session email opens collected for a
campaign.

WARNING: this field is deprecated, please use “emailUniqueOpen” instead. To ease up
the transition this field will still be available, but always return null.

### openRate:

WARNING: this field is deprecated, please use “emailUniqueOpenRate”.
To ease up the transition this field will still be available, but always return null.

### emailScheduled: !

Total emails scheduled to be sent as part if this campaign.

### emailSentUnconfirmed: !

Total emails attempted to be sent.

### emailBounced: !

Deliveries that were rejected by the recipient's email service provider.

### emailSentConfirmed: !

Total emails confirmed to have been sent by the Email Service Provider.

### emailDeliveryRate: !

The percent of emails that have been confirmed to be delivered, over the send attempts.

### emailMarkedSpam: !

Recipients who report your emails as spam.

### emailUniqueMarkedSpam: !

Recipients who report your emails as spam, uniqued.

### emailUniqueOpen: !

When an email is opened by a user in its lifetime.

### emailUniqueOpenRate: !

The percent of sent emails that are opened once in a user's lifetime.

### emailUniqueClick: !

The number of times a link in an email was clicked once in a user's lifetime.

### emailUniqueClickRate: !

The percentage of emails opened that were clicked once in a user's lifetime.

### emailUniqueUnsubscribers: !

Recipients that unsubscribe from the email list, uniqued.

### emailUniqueUnsubscribeRate: !

The percent of recipients that have unsubscribers (unique) over the number of confirmed to be deliveries.

### emailUnsubscribers: !

Recipients that unsubscribe from the email list

### emailUniqueClicksByCountry:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times an email was clicked once in a user's lifetime broken out by ISO-2 country code

### emailUniqueOpensByCountry:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times an email is opened by a user in its lifetime, broken out by ISO-2 country code

### emailUniqueClicksByDeviceType:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times a link in an email was clicked once in a user's lifetime, broken out by device type
One of ‘pc’, ‘mobile’, ‘tablet’, ‘other’.

### emailUniqueOpensByDeviceType:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Number of times an email is opened by a user in its lifetime, broken out by device type
One of ‘pc’, ‘mobile’, ‘tablet’, ‘other’.

### emailUniqueClicksByXpathUrl:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Unique clicks by xpath;url present in an email message
The key <xpath>;<url or macro> consists in 2 parts:
1. A XPath locator to the individual element that was clicked in the email message, based on a HTML5-compliant tree.
2. URL or macro: either a static URL that was clicked present in the email template or, the macro used to generate the URL. Eg.: {{product.url}}. Useful to identify links generated for the same intent, but it might show differently for emailed contacts.

In the future we may break this out to seperate metrics

### smsSentDelivered: !

Total number of SMS messages that were delivered (and confirmed by the recipient)

### smsClicks: !

Total number of times that a link in the SMS message was clicked.

### videoImpressions:

Impressions from video ads.

### videoViews:

Number of times the video begun playing.

### videoTwentyFivePercent:

Number of times at least 25% of the video duration was played.

### videoFiftyPercent:

Number of times at least 50% of the video duration was played.

### videoSeventyFivePercent:

Number of times at least 75% of the video duration was played.

### videoHundredPercent:

Number of times the full video duration was played.

### videoCompletionRate:

Video completion rate

Video Completion Rate (x) = Video Viewed To 100% / Video Impressions

### frequency: !

Number of ads seen per day by reached users (only applies to WEB campaigns)

Frequency = total impressions/reached users

### deviceFrequency: !

Number of ads seen per day by reached devices (only applies to CTV campaigns)

Device Frequency = total impressions/reached devices

### totalUniqueHHsReached:

Number of distinct households that received CTV impressions on a given day

### uniqueHHSiteVisits:

Number of distinct households that visited the site, after viewing an ad

### siteBounceRate:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteNewVisitors:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteEngaged:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteEngagedNewVisitors:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### siteAddToCart:

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

### customMetric(formula:) : !

[ALPHA] This GraphQL field is currently under development and QA, please
hold off from using it. It might change or be removed in the future,
within this API’s version.

Usage:
- Operators: ‘+’, ‘-’, ‘\*’, ‘/’ and parentheses () are valid
Requires formula to have space-seperated operand and operators.

e.g. costPerImpression: customMetric(formula: “cost / impressions”)

**Arguments**:

### formula:

### MetricResult

Groups reporting metric data in summary and by date format.

**Fields**:

### summary: !

Summarizes the reporting data for the given date range.

### byDate: [!]!

Reporting data by date in the given range.

### Organization

**Fields**:

### eid: !

EID of the organization.

### name: !

Name of the organization.

### createdDate:

Created date for the organization.

### advertisables: [!]!

Advertisables for the current organization.

### metricsTotal:

Provides aggregation for any metrics in the current and child
nodes.

Note that this will not load the metrics by itself, instead it
aggregates loaded metrics fields in its scope.

For details see the documentation of MetricAggregateResult.

### OrganizationGroupData

**Fields**:

### eid: !

EID of the organization.

### name: !

Name of the organization.

### createdDate:

Created date for the organization.

### OrganizationQuery

**Fields**:

### byEID(organization: !):

Obtain an Organization by its unique identifier (EID).

**Arguments**:

### organization: !

Organization EID.

### byEIDs(eids: [!]!): []!

Obtain a list of Organizations by their unique identifiers (EID).

**Arguments**:

### eids: [!]!

List of Organization EIDs.

### current:

Obtain the Organization the current user is part of.

### metricsTotal:

Provides aggregation for any metrics in the current and child
nodes.

Note that this will not load the metrics by itself, instead it
aggregates loaded metrics fields in its scope.

For details see the documentation of MetricAggregateResult.

### PerformanceTarget

**Fields**:

### metric: !

### currencyCode: !

### goal: !

### Placement

Contains reporting metric data for attributions, deliveries

by placement.

**Fields**:

### placement: !

Placement of the Ad in Facebook. For example ‘desktop’, ‘feed’…

### impressions: !

The sum of the number of ad impressions.

### clicks: !

The sum of clicks of all kinds of ads and emails.

### cost: !

Cost associated to all kinds of ads and emails.

### conversions: !

Conversions
Total.
Conversions (count) = View Conversions + Click Conversions

### clickThroughs: !

Click-through conversion (CTC).
A goal completion that happens after someone clicks your ad.

### viewThroughs: !

View-through conversion (VTC).
A goal completion that happens after someone views your ad, but
does not click.

### revenue: !

Revenue (amount) = View Revenue + Click Conversions

### clickRevenue: !

Click-Attributed Revenue.
Total earnings when someone clicks your ad and converts.

### viewRevenue: !

View-Attributed Revenue.
Total earnings when someone views your ad and converts.

### ctr: !

Click-through rate.
The percentage of ad serves that were clicked.

CTR (%) = Clicks / Impression \* 100

### cpc: !

Cost per click.
Your average spend for one click.

CPC ($) = Spend / Clicks

### cpm: !

Cost per mille.
Cost per one thousand ad serves.

CPM ($) = Spend / Impressions \* 1000

### cpa: !

Cost per acquisition.
Your average spend per conversion.

CPA ($) = Spend / Conversions

### clickCPA: !

Cost-per-click acquisition.
Your average spend for a conversion that happens after someone clicks your ad.

Click CPA ($) = Spend / Click Conversions

### viewCPA: !

Cost-per-view acquisition: Your average spend for a
conversion that happens after someone views your ad.

View CPA ($) = Cost / View Throughs

### averageOrderValue: !

Average Order Value
Average revenue per attributed conversion.

Average Order Value ($) = Attributed Revenue / Conversions

### ctcRate: !

Click-through conversion rate.
The percentage of clicks that resulted in a click-through conversion.

CTC Rate (%) = Click Conversions / Clicks \* 100

### vtcRate: !

View-through conversion rate: The percentage of impressions
that resulted in a view-through conversion.

VTC Rate (%) = View Throughs / Impressions \* 100

### roas: !

Return on advertising spend: Your profit per dollar spent
on ads.

ROAS (x) = (Click Revenue + View Revenue) / Cost

### clickROAS: !

Click return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone clicks
your ad.

Click ROAS (x) = Click Revenue / Cost

### viewROAS: !

View return on advertising spend: Your profit per dollar spent,
generated from conversions that happen after someone views
your ad.

View ROAS (x) = View Revenue / Cost

### roi: !

Alias for ‘roas’.

### clickROI: !

Alias for ‘clickROAS’.

### viewROI: !

Alias for ‘viewROAS’.

### PlacementResult

Groups reporting metric data in summary and by date format.

**Fields**:

### byPlacement: [!]!

Summarizes by placement the reporting data for the given date range.

### Query

Root element for a Reporting API GraphQL’s query.

**Fields**:

### flags(enableAdcrabLabels: !, enableKlaviyoFlowCampaigns: !, enableUniversalCampaigns: !, enableProxyCampaigns: !, enablePinterestCampaigns: !, enableTikTokCampaigns: !, enableGoogleSearchCampaigns: !, enableMultiChannelCampaigns: !, enableConnectedTVCampaigns: !, enableSMSCampaigns: !, enableObjectiveLedCampaigns: !, listOnlyInventoryForVoltronStrategies: !, useExperimentalProxyCampaigns: !, includeExpiredData: !, useAdrollAdsStatusOnlyEndpoint: !, useAdcrabDimensionsForSize: !, useOnlyCostMetricsUhura: !, stripNullValues: !, useSemanticLayer: !): !

Setup global request flags

**Arguments**:

### enableAdcrabLabels: !

Include custom labels data for Ads.
Labels are requested from the Adcrab API.
For internal use only.

* **Default:**
  false

### enableKlaviyoFlowCampaigns: !

Includes Flows for Klaviyo Email campaigns.
The enableMultiChannelCampaigns flag must be enabled as well.
For internal use only.

* **Default:**
  false

### enableUniversalCampaigns: !

Enables or disables fetching Universal campaigns for
advertisable and organization queries and filtering of
inventory campaigns. This does not affect queries
using EIDs.

Note: The default value for this flag will be changed to
true once universal campaign support is considered
stable.

* **Default:**
  false

### enableProxyCampaigns: !

Enables or disables fetching Proxy campaigns for
advertisable and organization queries and filtering of
inventory campaigns.

This does not affect queries using EIDs.

* **Default:**
  false

### enablePinterestCampaigns: !

Include experimental Pinterest Connected Ads campaigns.
For internal use only.

* **Default:**
  false

### enableTikTokCampaigns: !

Include experimental TikTok Connected Ads campaigns.
For internal use only.

* **Default:**
  false

### enableGoogleSearchCampaigns: !

Include experimental Google Search Connected Ads campaigns.
For internal use only.

* **Default:**
  false

### enableMultiChannelCampaigns: !

Include experimental MultiChannel Connected Ads campaigns.
For internal use only.

* **Default:**
  false

### enableConnectedTVCampaigns: !

Include experimental Connected TV Ads campaigns.

* **Default:**
  false

### enableSMSCampaigns: !

Include experimental SMS campaigns.
For internal use only.

* **Default:**
  false

### enableObjectiveLedCampaigns: !

Even if not requested, enables or disables loading Ad Groups.
Ad Group data is required for Objective Led Campaigns Targeting.
For internal use only.

* **Default:**
  false

### listOnlyInventoryForVoltronStrategies: !

> When enableProxyCampaigns or enableUniversalCampaigns is enabled,

return just the inventory campaigns filtering out the top-level
proxy or UC campaigns. Does not apply to Playbooks.

> This flag is used by reports to avoid duplicating metric numbers
> when both the top-level and inventory campaigns are included in the
> results.
* **Default:**
  false

### useExperimentalProxyCampaigns: !

For internal use only. Don’t use it, it will disappear soon with no warning.

* **Default:**
  false

### includeExpiredData: !

Exclude data that is no longer relevant. When set to false it will:
- Drop entities that were deleted more than 3 months ago.
- Limit metric data to the last 3 years.

* **Default:**
  true

### useAdrollAdsStatusOnlyEndpoint: !

When useAdrollAdsStatusOnlyEndpoint is enabled, only ads status data will be fetched.
non-status-related field arguments such as ads(width=int) will not work given that
this ad data will not be retrieved.

* **Default:**
  false

### useAdcrabDimensionsForSize: !

When useAdcrabDimensionsForSize is enabled, width and height will be retrieved from AdCrab.

* **Default:**
  false

### useOnlyCostMetricsUhura: !

When useOnlyCostMetricsUhura is enabled a only_cost_metrics flag will be added to the Uhura deliveries query
Only campaign eids, advertisable eids, and cost metrics will be returned from the endpoint.
This means that the deliveries query will not return any other metrics such as impressions, clicks, etc.
This also means that the deliveries query will not return any adgroup or ad data, only campaign cost data.
This was added to increase performance for large datasets where only cost metrics are needed.

* **Default:**
  false

### stripNullValues: !

For Internal use only. When stripNullValues is enabled, null values will be removed from the response.

* **Default:**
  false

### useSemanticLayer: !

For internal use only. When useSemanticLayer is enabled, it will instruct the reporting API to fetch data from
an experimental semantic layer. This flag will be removed with no warning.

* **Default:**
  false

### requestId: !

Unique ID for this request. This can be used to retrieve debugging
and profiling info for the request.

### build: !

Reporting API build number and environment.

### organization: !

Root for querying Organizations.

### advertisable: !

Root for querying Advertisables.

### campaign: !

Root for querying Campaigns.

### adgroup: !

Root for querying Adgroups.

### ad: !

Root for querying Ads.

### automation: !

Root for querying Automation.

### email: !

Root for querying Emails.

### segment:

Use the child Audiences of Campaigns and AdGroups instead.

Root for querying Segments.

### group:

[BETA] This GraphQL node is currently under development.
Avoid its use in production until it has passed some thorough QA.

Provides custom grouping in queries.

### user: !

Currently logged user.

### actualUser: !

Currently logged actual user.

### metricsTotal:

Provides aggregation for any metrics in the current and child
nodes.

Note that this will not load the metrics by itself, instead it
aggregates loaded metrics fields in its scope.

For details see the documentation of MetricAggregateResult.

### accountMetrics:

[ALPHA] This GraphQL node is currently under development
Avoid its use in production until it has passed some thorough QA.

Provides metrics per account for a list of campaigns and an advertisable,
over a specific date range.
It will return the metrics for the top 1000 accounts by spend.

### log: [!]!

[WARNING] Log lines are intended for internal analysis and debugging.
They are not available for external developers to consume.

Return log entries for the current query.

### logSchema: [!]!

[WARNING] Log lines are intended for internal analysis and debugging.
They are not available for external developers to consume.

Return log messages generated by the schema compilation.

### queryLog:

Available only for internal developers.

### Segment

**Fields**:

### eid: !

The Segment EID.

### name: !

The Segment Name.

### duration: !

The Segment’s duration in days.

### isActive: !

False if the segment has been deleted.

### isConversion: !

True if this is a conversion segment.

### type: !

Segment type.

### tags: !

Tags explicitly assigned to the segment.

### conversionValue: !

The value of a conversion from this segment.

### currency: !

The value of a conversion from this segment. Default to the
Advertisable’s currency.

### description: !

Pieces to build the Segment’s description formatted following the type.

### product:

Product the segment belongs to.

### SegmentGroupData

**Fields**:

### eid: !

The Segment EID.

### name: !

The Segment Name.

### duration: !

The Segment’s duration in days.

### isActive: !

False if the segment has been deleted.

### isConversion: !

True if this is a conversion segment.

### type: !

Segment type.

### tags: !

Tags explicitly assigned to the segment.

### conversionValue: !

The value of a conversion from this segment.

### currency: !

The value of a conversion from this segment. Default to the
Advertisable’s currency.

### description: !

Pieces to build the Segment’s description formatted following the type.

### product:

Product the segment belongs to.

### SegmentQuery

**Fields**:

### byEID(segment: !):

[WARNING] Fetching Segments directly through this operation will
ignore the overrides and state provided by its relationship to an
AdGroup. For a complete state fetch segments as children of
Campaigns or AdGroups.

**Arguments**:

### segment: !

Resolves a Segment by its EID.

### byEIDs(eids: [!]!): []!

[WARNING] Fetching Segments directly through this operation will
ignore the overrides and state provided by its relationship to an
AdGroup. For a complete state fetch segments as children of
Campaigns or AdGroups.

**Arguments**:

### eids: [!]!

Resolves multiple Segments by their EID.

### byAdvertisable(advertisable: !, isActive: , isConversion:) : []!

[WARNING] Fetching Segments directly through this operation will
ignore the overrides and state provided by its relationship to an
AdGroup. For a complete state fetch segments as children of
Campaigns or AdGroups.

**Arguments**:

### advertisable: !

Required advertisable EID.

### isActive:

If True, only active segments will be returned, and vice versa (Optional; default: False)

### isConversion:

If True, only conversion segments will be returned (Optional; default: False).

### User

Provides information about a logged user.

**Fields**:

### eid: !

User EID.

### isActive: !

Is the user active?

### status: !

User’s status.

### email: !

User’s email.

### userName: !

User’s login name.

### name: !

Full user name

### firstName: !

User’s first name.

### lastName: !

User’s last name.

### advertisables: [!]

List of user advertisables.

### organization: !

The organization the user belongs to.

### locale: !

User’s locale.

### defaultTimezone: !

Default timezone for the user.

### createdDate:

Date the user was created.

### role: !

User’s role.

### hasPermission(name:) : !

Is true if the user has the given permission.

**Arguments**:

### name:

### permissions: [!]

Full list of user’s permissions.

### isInternal: !

Is true if the user is considered an internal user. This is based
on the user’s permissions.

### UtmBasedConversionsForAdvertisable

Contains advertisable-level UTM-based conversions data.

**Fields**:

### utm: !

### aov: !

### assistConversions: !

### assistRevenue: !

### assistAov: !

### conversions: !

### revenue: !

### campaigns: [!]!

Campaign level data.

### UtmBasedConversionsForCampaign

Contains campaign-level UTM-based conversions data.

**Fields**:

### campaignEID:

### utm: !

### aov: !

### assistConversions: !

### assistRevenue: !

### assistAov: !

### conversions: !

### revenue: !

## Scalars

Scalars represent primitive types and cannot have fields.

### List

- [`Boolean`](#Boolean)
- [`Date`](#Date)
- [`DateTime`](#DateTime)
- [`Decimal`](#Decimal)
- [`Float`](#Float)
- [`ID`](#ID)
- [`Int`](#Int)
- [`JSON`](#JSON)
- [`String`](#String)

### Descriptions

### Boolean

The Boolean scalar type represents true or false.

### Date

Scalar type for dates.

### DateTime

Scalar type for dates with time information.

### Decimal

Scalar type for decimal numeric values.

### Float

The Float scalar type represents signed double‐precision fractional values as specified by IEEE 754.

### ID

The ID scalar type represents a unique identifier, often used to refetch an object or as the key for a cache.

### Int

The Int scalar type represents a signed 32‐bit numeric non‐fractional value.

### JSON

Scalar type for arbitrary JSON data.

### String

The String scalar type represents textual data, represented as UTF‐8 character sequences.
