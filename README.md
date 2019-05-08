# ![LOGO](logo.png) SportsData **flow**ground Connector

## Description

A generated **flow**ground connector for the SportsData API (version 2).

Generated from: https://api.apis.guru/v2/specs/whapi.com/sportsdata/2/swagger.json<br/>
Generated at: 2019-05-07T17:44:54+03:00

## API Description

The William Hill SportsData REST API is a collection of GET methods to provide William Hill product data such as sport, competition, event, market and selection data (including prices).

## Authorization

This API does not require authorization.

## Actions

### Retrieves a list of competitions for a given class id.

*Tags:* `sportsdata`

#### Input Parameters
* `apiKey` - _required_ - Your API Key available from your developer portal
* `classId` - _required_ - The class id to retrieve information for.
* `isPublished` - _optional_ - Specify whether only active entities should be returned, according to the William Hill definition of active
* `fields` - _optional_ - Specify an absolute field list to return (Comma-Separated List)
* `include` - _optional_ - Specify fields in addition to the default to return (Comma-Separated List)
* `exclude` - _optional_ - Specify fields from the default to exclude (Comma-Separated List)
* `displayed` - _optional_ - Specify whether to return displayed entities or not
* `channel` - _optional_ - Specify a channel filter and only results from that channel will be returned
* `status` - _optional_ - Specify a status to filter results by. This is currently A (active) or S (suspended)
* `sort` - _optional_ - The field to order the response by, followed by the order. For example: name,desc
* `offset` - _optional_ - Skip over a number of elements by specifying a start value for the query
* `limit` - _optional_ - Specify the number of results to return
* `culture` - _optional_ - Code used to return responses in language other than English, acceptable values are de-DE|es-ES|fr-FR|nn-NO|fi-FI|ru-RU|pt-PT|hu-HU|sl-SL|ga-IE|en-CA|sr-Latn|sv-SE|el=GR|zh-CHS|it-IT|zh-CHT|cs-CZ|de-AT|ja-JP|pl-PL|da-DK|ro-RO|nl-NL|tr-TR

### Retrieves a list of events for a given class id.

> Retrieves a list of events for a given class id. 'includeAllDescendants' parameter should be accompanied with 'date' filter or one of 'dateFrom' and 'dateTo' filters.

*Tags:* `sportsdata`

#### Input Parameters
* `apiKey` - _required_ - Your API Key available from your developer portal
* `classId` - _required_ - The class id to retrieve information for.
* `isPublished` - _optional_ - Specify whether only active entities should be returned, according to the William Hill definition of active
* `fields` - _optional_ - Specify an absolute field list to return (Comma-Separated List)
* `include` - _optional_ - Specify fields in addition to the default to return (Comma-Separated List)
* `exclude` - _optional_ - Specify fields from the default to exclude (Comma-Separated List)
* `displayed` - _optional_ - Specify whether to return displayed entities or not
* `channel` - _optional_ - Specify a channel filter and only results from that channel will be returned
* `settled` - _optional_ - Specify wether only settled entities should be returned
* `includeEmpty` - _optional_ - When declared as false it should exclude markets and events that have no selections / markets
* `status` - _optional_ - Specify a status to filter results by. This is currently A (active) or S (suspended)
* `sort` - _optional_ - The field to order the response by, followed by the order. For example: name,desc
* `offset` - _optional_ - Skip over a number of elements by specifying a start value for the query
* `limit` - _optional_ - Specify the number of results to return
* `headlineSummary` - _optional_ - Return only headline markets (Markets with the lowest display order) Either 1 InPlay and 1 Pre-Match, or the amount specified in marketCount, if available. Markets and Outcomes will be returned.
* `includeAllDescendants` - _optional_ - Include every descendant in the below heirarchy
* `isInPlay` - _optional_ - Show only events that are in-play
* `marketCount` - _optional_ - Specify the number of markets to return when requesting headlineSummary. This count of InPlay and Pre-Match markets will be returned.For example, when specifying 1, 1 In Play and 1 Pre Match market will be returned.
* `date` - _optional_ - Return only events for the specified date (yyyy-MM-dd).
* `dateFrom` - _optional_ - The UTC datetime from the events to be returned. (yyyy-MM-ddTHH:mm:ss)
* `dateTo` - _optional_ - The UTC datetime TO the events to be returned. (yyyy-MM-ddTHH:mm:ss)
* `eventSort` - _optional_ - Filter event by event sort
* `culture` - _optional_ - Code used to return responses in language other than English, acceptable values are de-DE|es-ES|fr-FR|nn-NO|fi-FI|ru-RU|pt-PT|hu-HU|sl-SL|ga-IE|en-CA|sr-Latn|sv-SE|el=GR|zh-CHS|it-IT|zh-CHT|cs-CZ|de-AT|ja-JP|pl-PL|da-DK|ro-RO|nl-NL|tr-TR
* `marketPublished` - _optional_ - Specify whether only active entities should be returned, according to the William Hill definition of active
* `marketStatus` - _optional_ - Specify a status to filter results by. This is currently A (active) or S (suspended)
* `marketDisplayed` - _optional_ - Specify whether to return displayed entities or not
* `marketChannel` - _optional_ - Specify a channel filter and only results from that channel will be returned
* `marketSort` - _optional_ - Filter by market sort (e.g. MR (match result) -- (Outright)).
* `marketEW` - _optional_ - Specify whether to return markets with each way betting or those without
* `selectionStatus` - _optional_ - Specify a status to filter results by. This is currently A (active) or S (suspended)
* `selectionChannel` - _optional_ - Specify a channel filter and only results from that channel will be returned
* `selectionPublished` - _optional_ - Specify whether only active entities should be returned, according to the William Hill definition of active

### Retrieves a specific competition

*Tags:* `sportsdata`

#### Input Parameters
* `apiKey` - _required_ - Your API Key available from your developer portal
* `competitionId` - _required_ - The competition id to retrieve information for.
* `fields` - _optional_ - Specify an absolute field list to return (Comma-Separated List)
* `include` - _optional_ - Specify fields in addition to the default to return (Comma-Separated List)
* `exclude` - _optional_ - Specify fields from the default to exclude (Comma-Separated List)
* `culture` - _optional_ - Code used to return responses in language other than English, acceptable values are de-DE|es-ES|fr-FR|nn-NO|fi-FI|ru-RU|pt-PT|hu-HU|sl-SL|ga-IE|en-CA|sr-Latn|sv-SE|el=GR|zh-CHS|it-IT|zh-CHT|cs-CZ|de-AT|ja-JP|pl-PL|da-DK|ro-RO|nl-NL|tr-TR

### Retrieves a list of events for a given competition id.

> Retrieves a list of events for a given competition id. 'headlineSummary' and includeAllDescendants parameters should be accompanied with 'date' filter or one of 'dateFrom' and 'dateTo' filters.

*Tags:* `sportsdata`

#### Input Parameters
* `apiKey` - _required_ - Your API Key available from your developer portal
* `competitionId` - _required_ - The competition id to retrieve information for.
* `isPublished` - _optional_ - Specify whether only active entities should be returned, according to the William Hill definition of active
* `fields` - _optional_ - Specify an absolute field list to return (Comma-Separated List)
* `include` - _optional_ - Specify fields in addition to the default to return (Comma-Separated List)
* `exclude` - _optional_ - Specify fields from the default to exclude (Comma-Separated List)
* `displayed` - _optional_ - Specify whether to return displayed entities or not
* `channel` - _optional_ - Specify a channel filter and only results from that channel will be returned
* `settled` - _optional_ - Specify wether only settled entities should be returned
* `includeEmpty` - _optional_ - When declared as false it should exclude markets and events that have no selections / markets
* `status` - _optional_ - Specify a status to filter results by. This is currently A (active) or S (suspended)
* `sort` - _optional_ - The field to order the response by, followed by the order. For example: name,desc
* `offset` - _optional_ - Skip over a number of elements by specifying a start value for the query
* `limit` - _optional_ - Specify the number of results to return
* `headlineSummary` - _optional_ - Return only headline markets (Markets with the lowest display order) Either 1 InPlay and 1 Pre-Match, or the amount specified in marketCount, if available. Markets and Outcomes will be returned.
* `includeAllDescendants` - _optional_ - Include every descendant in the below heirarchy
* `isInPlay` - _optional_ - Show only events that are in-play
* `marketCount` - _optional_ - Specify the number of markets to return when requesting headlineSummary. This count of InPlay and Pre-Match markets will be returned.For example, when specifying 1, 1 In Play and 1 Pre Match market will be returned.
* `date` - _optional_ - Return only events for the specified date (yyyy-MM-dd).
* `dateFrom` - _optional_ - The UTC datetime from the events to be returned. (yyyy-MM-ddTHH:mm:ss)
* `dateTo` - _optional_ - The UTC datetime TO the events to be returned. (yyyy-MM-ddTHH:mm:ss)
* `marketGroupId` - _optional_ - Filter by marketGroupId (e.g. OB_MG1276585).
* `eventSort` - _optional_ - Filter event by event sort
* `culture` - _optional_ - Code used to return responses in language other than English, acceptable values are de-DE|es-ES|fr-FR|nn-NO|fi-FI|ru-RU|pt-PT|hu-HU|sl-SL|ga-IE|en-CA|sr-Latn|sv-SE|el=GR|zh-CHS|it-IT|zh-CHT|cs-CZ|de-AT|ja-JP|pl-PL|da-DK|ro-RO|nl-NL|tr-TR
* `marketPublished` - _optional_ - Specify whether only active entities should be returned, according to the William Hill definition of active
* `marketStatus` - _optional_ - Specify a status to filter results by. This is currently A (active) or S (suspended)
* `marketDisplayed` - _optional_ - Specify whether to return displayed entities or not
* `marketChannel` - _optional_ - Specify a channel filter and only results from that channel will be returned
* `marketSort` - _optional_ - Filter by market sort (e.g. MR (match result) -- (Outright)).
* `marketEW` - _optional_ - Specify whether to return markets with each way betting or those without
* `selectionStatus` - _optional_ - Specify a status to filter results by. This is currently A (active) or S (suspended)
* `selectionChannel` - _optional_ - Specify a channel filter and only results from that channel will be returned
* `selectionPublished` - _optional_ - Specify whether only active entities should be returned, according to the William Hill definition of active

### Retrieves a list of market groups for a given competition id

*Tags:* `sportsdata`

#### Input Parameters
* `apiKey` - _required_ - Your API Key available from your developer portal
* `competitionId` - _required_ - The competition id to retrieve information for.
* `fields` - _optional_ - Specify an absolute field list to return (Comma-Separated List)
* `include` - _optional_ - Specify fields in addition to the default to return (Comma-Separated List)
* `exclude` - _optional_ - Specify fields from the default to exclude (Comma-Separated List)
* `sort` - _optional_ - The field to order the response by, followed by the order. For example: name,desc
* `offset` - _optional_ - Skip over a number of elements by specifying a start value for the query
* `limit` - _optional_ - Specify the number of results to return
* `culture` - _optional_ - Code used to return responses in language other than English, acceptable values are de-DE|es-ES|fr-FR|nn-NO|fi-FI|ru-RU|pt-PT|hu-HU|sl-SL|ga-IE|en-CA|sr-Latn|sv-SE|el=GR|zh-CHS|it-IT|zh-CHT|cs-CZ|de-AT|ja-JP|pl-PL|da-DK|ro-RO|nl-NL|tr-TR
* `name` - _optional_ - Filter by market group name

### Retrieves a list of events for the provided IDs.

*Tags:* `sportsdata`

#### Input Parameters
* `apiKey` - _required_ - Your API Key available from your developer portal
* `ids` - _optional_ - A comma-separated list of selectionIds
* `isPublished` - _optional_ - Specify whether only active entities should be returned, according to the William Hill definition of active
* `includeAllDescendants` - _optional_ - Include every descendant in the below heirarchy
* `fields` - _optional_ - Specify an absolute field list to return (Comma-Separated List)
* `include` - _optional_ - Specify fields in addition to the default to return (Comma-Separated List)
* `exclude` - _optional_ - Specify fields from the default to exclude (Comma-Separated List)
* `channel` - _optional_ - Specify a channel filter and only results from that channel will be returned
* `settled` - _optional_ - Specify wether only settled entities should be returned
* `includeEmpty` - _optional_ - When declared as false it should exclude markets and events that have no selections / markets
* `headlineSummary` - _optional_ - Return only headline markets (Markets with the lowest display order) Either 1 InPlay and 1 Pre-Match, or the amount specified in marketCount, if available. Markets and Outcomes will be returned.
* `marketCount` - _optional_ - Specify the number of markets to return when requesting headlineSummary. This count of InPlay and Pre-Match markets will be returned.For example, when specifying 1, 1 In Play and 1 Pre Match market will be returned.
* `sort` - _optional_ - The field to order the response by, followed by the order. For example: name,desc
* `offset` - _optional_ - Skip over a number of elements by specifying a start value for the query
* `limit` - _optional_ - Specify the number of results to return
* `marketIds` - _optional_ - Comma-seaerated list of market IDs to filter by
* `culture` - _optional_ - Code used to return responses in language other than English, acceptable values are de-DE|es-ES|fr-FR|nn-NO|fi-FI|ru-RU|pt-PT|hu-HU|sl-SL|ga-IE|en-CA|sr-Latn|sv-SE|el=GR|zh-CHS|it-IT|zh-CHT|cs-CZ|de-AT|ja-JP|pl-PL|da-DK|ro-RO|nl-NL|tr-TR
* `marketPublished` - _optional_ - Specify whether only active entities should be returned, according to the William Hill definition of active
* `marketStatus` - _optional_ - Specify a status to filter results by. This is currently A (active) or S (suspended)
* `marketDisplayed` - _optional_ - Specify whether to return displayed entities or not
* `marketChannel` - _optional_ - Specify a channel filter and only results from that channel will be returned
* `marketSort` - _optional_ - Filter by market sort (e.g. MR (match result) -- (Outright)).
* `marketEW` - _optional_ - Specify whether to return markets with each way betting or those without
* `selectionStatus` - _optional_ - Specify a status to filter results by. This is currently A (active) or S (suspended)
* `selectionChannel` - _optional_ - Specify a channel filter and only results from that channel will be returned
* `selectionPublished` - _optional_ - Specify whether only active entities should be returned, according to the William Hill definition of active

### Retrieves a single event by ID.

*Tags:* `sportsdata`

#### Input Parameters
* `apiKey` - _required_ - Your API Key available from your developer portal
* `eventId` - _required_ - The event ID to retrieve information for.
* `includeAllDescendants` - _optional_ - Include every descendant in the below heirarchy
* `fields` - _optional_ - Specify an absolute field list to return (Comma-Separated List)
* `include` - _optional_ - Specify fields in addition to the default to return (Comma-Separated List)
* `exclude` - _optional_ - Specify fields from the default to exclude (Comma-Separated List)
* `headlineSummary` - _optional_ - Return only headline markets (Markets with the lowest display order) Either 1 InPlay and 1 Pre-Match, or the amount specified in marketCount, if available. Markets and Outcomes will be returned.
* `marketCount` - _optional_ - Specify the number of markets to return when requesting headlineSummary. This count of InPlay and Pre-Match markets will be returned.For example, when specifying 1, 1 In Play and 1 Pre Match market will be returned.
* `marketIds` - _optional_ - Comma-seaerated list of market IDs to filter by
* `includeEmpty` - _optional_ - When declared as false it should exclude markets and events that have no selections / markets
* `culture` - _optional_ - Code used to return responses in language other than English, acceptable values are de-DE|es-ES|fr-FR|nn-NO|fi-FI|ru-RU|pt-PT|hu-HU|sl-SL|ga-IE|en-CA|sr-Latn|sv-SE|el=GR|zh-CHS|it-IT|zh-CHT|cs-CZ|de-AT|ja-JP|pl-PL|da-DK|ro-RO|nl-NL|tr-TR
* `marketPublished` - _optional_ - Specify whether only active entities should be returned, according to the William Hill definition of active
* `marketStatus` - _optional_ - Specify a status to filter results by. This is currently A (active) or S (suspended)
* `marketDisplayed` - _optional_ - Specify whether to return displayed entities or not
* `marketChannel` - _optional_ - Specify a channel filter and only results from that channel will be returned
* `marketSort` - _optional_ - Filter by market sort (e.g. MR (match result) -- (Outright)).
* `marketEW` - _optional_ - Specify whether to return markets with each way betting or those without
* `selectionStatus` - _optional_ - Specify a status to filter results by. This is currently A (active) or S (suspended)
* `selectionChannel` - _optional_ - Specify a channel filter and only results from that channel will be returned
* `selectionPublished` - _optional_ - Specify whether only active entities should be returned, according to the William Hill definition of active

### Retrieves competitors for a single event by ID.

*Tags:* `competitors`

#### Input Parameters
* `apiKey` - _required_ - Your API Key available from your developer portal
* `eventId` - _required_ - The event ID to retrieve information for.
* `fields` - _optional_ - Specify an absolute field list to return (Comma-Separated List)
* `include` - _optional_ - Specify fields in addition to the default to return (Comma-Separated List)
* `exclude` - _optional_ - Specify fields from the default to exclude (Comma-Separated List)

### Gets one or more specific markets

> Retrieves one or more specific markets. Markets with Live at the end are always In-Play markets. However, not ALL In-Play markets have Live at the end of the market name.

*Tags:* `sportsdata`

#### Input Parameters
* `apiKey` - _required_ - Your API Key available from your developer portal
* `eventId` - _required_ - The event ID to retrieve information for.
* `ids` - _optional_ - A comma-separated list of selectionIds
* `includeAllDescendants` - _optional_ - Include every descendant in the below heirarchy
* `fields` - _optional_ - Specify an absolute field list to return (Comma-Separated List)
* `include` - _optional_ - Specify fields in addition to the default to return (Comma-Separated List)
* `exclude` - _optional_ - Specify fields from the default to exclude (Comma-Separated List)
* `includeEmpty` - _optional_ - When declared as false it should exclude markets and events that have no selections / markets
* `culture` - _optional_ - Code used to return responses in language other than English, acceptable values are de-DE|es-ES|fr-FR|nn-NO|fi-FI|ru-RU|pt-PT|hu-HU|sl-SL|ga-IE|en-CA|sr-Latn|sv-SE|el=GR|zh-CHS|it-IT|zh-CHT|cs-CZ|de-AT|ja-JP|pl-PL|da-DK|ro-RO|nl-NL|tr-TR
* `marketPublished` - _optional_ - Specify whether only active entities should be returned, according to the William Hill definition of active
* `marketStatus` - _optional_ - Specify a status to filter results by. This is currently A (active) or S (suspended)
* `marketDisplayed` - _optional_ - Specify whether to return displayed entities or not
* `marketChannel` - _optional_ - Specify a channel filter and only results from that channel will be returned
* `marketSort` - _optional_ - Filter by market sort (e.g. MR (match result) -- (Outright)).
* `marketEW` - _optional_ - Specify whether to return markets with each way betting or those without
* `selectionStatus` - _optional_ - Specify a status to filter results by. This is currently A (active) or S (suspended)
* `selectionChannel` - _optional_ - Specify a channel filter and only results from that channel will be returned
* `selectionPublished` - _optional_ - Specify whether only active entities should be returned, according to the William Hill definition of active

### Gets one or more selections for a market

> Retrieves one or more selections for a market

*Tags:* `sportsdata`

#### Input Parameters
* `apiKey` - _required_ - Your API Key available from your developer portal
* `eventId` - _required_ - The event ID to retrieve information for.
* `marketId` - _required_ - The market id to retrieve information for
* `ids` - _optional_ - A comma-separated list of selectionIds
* `fields` - _optional_ - Specify an absolute field list to return (Comma-Separated List)
* `include` - _optional_ - Specify fields in addition to the default to return (Comma-Separated List)
* `exclude` - _optional_ - Specify fields from the default to exclude (Comma-Separated List)
* `culture` - _optional_ - Code used to return responses in language other than English, acceptable values are de-DE|es-ES|fr-FR|nn-NO|fi-FI|ru-RU|pt-PT|hu-HU|sl-SL|ga-IE|en-CA|sr-Latn|sv-SE|el=GR|zh-CHS|it-IT|zh-CHT|cs-CZ|de-AT|ja-JP|pl-PL|da-DK|ro-RO|nl-NL|tr-TR
* `selectionStatus` - _optional_ - Specify a status to filter results by. This is currently A (active) or S (suspended)
* `selectionChannel` - _optional_ - Specify a channel filter and only results from that channel will be returned
* `selectionPublished` - _optional_ - Specify whether only active entities should be returned, according to the William Hill definition of active

### Gets a list of all sports

*Tags:* `sportsdata`

#### Input Parameters
* `apiKey` - _required_ - Your API Key available from your developer portal
* `sort` - _optional_ - The field to order the response by, followed by the order. For example: name,desc
* `offset` - _optional_ - Skip over a number of elements by specifying a start value for the query
* `isPublished` - _optional_ - Specify whether only active entities should be returned, according to the William Hill definition of active
* `limit` - _optional_ - Specify the number of results to return
* `fields` - _optional_ - Specify an absolute field list to return (Comma-Separated List)
* `include` - _optional_ - Specify fields in addition to the default to return (Comma-Separated List)
* `exclude` - _optional_ - Specify fields from the default to exclude (Comma-Separated List)
* `culture` - _optional_ - Code used to return responses in language other than English, acceptable values are de-DE|es-ES|fr-FR|nn-NO|fi-FI|ru-RU|pt-PT|hu-HU|sl-SL|ga-IE|en-CA|sr-Latn|sv-SE|el=GR|zh-CHS|it-IT|zh-CHT|cs-CZ|de-AT|ja-JP|pl-PL|da-DK|ro-RO|nl-NL|tr-TR

### Retrieves a list of classes for a given sport id.

*Tags:* `sportsdata`

#### Input Parameters
* `apiKey` - _required_ - Your API Key available from your developer portal
* `sportId` - _required_ - The sport id to retrieve information for.
* `isPublished` - _optional_ - Specify whether only active entities should be returned, according to the William Hill definition of active
* `fields` - _optional_ - Specify an absolute field list to return (Comma-Separated List)
* `include` - _optional_ - Specify fields in addition to the default to return (Comma-Separated List)
* `exclude` - _optional_ - Specify fields from the default to exclude (Comma-Separated List)
* `displayed` - _optional_ - Specify whether to return displayed entities or not
* `channel` - _optional_ - Specify a channel filter and only results from that channel will be returned
* `status` - _optional_ - Specify a status to filter results by. This is currently A (active) or S (suspended)
* `sort` - _optional_ - The field to order the response by, followed by the order. For example: name,desc
* `offset` - _optional_ - Skip over a number of elements by specifying a start value for the query
* `limit` - _optional_ - Specify the number of results to return
* `culture` - _optional_ - Code used to return responses in language other than English, acceptable values are de-DE|es-ES|fr-FR|nn-NO|fi-FI|ru-RU|pt-PT|hu-HU|sl-SL|ga-IE|en-CA|sr-Latn|sv-SE|el=GR|zh-CHS|it-IT|zh-CHT|cs-CZ|de-AT|ja-JP|pl-PL|da-DK|ro-RO|nl-NL|tr-TR

### Retrieves a list of competitions for a given sport id.

*Tags:* `sportsdata`

#### Input Parameters
* `apiKey` - _required_ - Your API Key available from your developer portal
* `sportId` - _required_ - The sport id to retrieve information for.
* `isPublished` - _optional_ - Specify whether only active entities should be returned, according to the William Hill definition of active
* `fields` - _optional_ - Specify an absolute field list to return (Comma-Separated List)
* `include` - _optional_ - Specify fields in addition to the default to return (Comma-Separated List)
* `exclude` - _optional_ - Specify fields from the default to exclude (Comma-Separated List)
* `displayed` - _optional_ - Specify whether to return displayed entities or not
* `channel` - _optional_ - Specify a channel filter and only results from that channel will be returned
* `status` - _optional_ - Specify a status to filter results by. This is currently A (active) or S (suspended)
* `sort` - _optional_ - The field to order the response by, followed by the order. For example: name,desc
* `offset` - _optional_ - Skip over a number of elements by specifying a start value for the query
* `limit` - _optional_ - Specify the number of results to return
* `culture` - _optional_ - Code used to return responses in language other than English, acceptable values are de-DE|es-ES|fr-FR|nn-NO|fi-FI|ru-RU|pt-PT|hu-HU|sl-SL|ga-IE|en-CA|sr-Latn|sv-SE|el=GR|zh-CHS|it-IT|zh-CHT|cs-CZ|de-AT|ja-JP|pl-PL|da-DK|ro-RO|nl-NL|tr-TR

### Retrieves a weighted list of Selections.

*Tags:* `sportsdata`

#### Input Parameters
* `apiKey` - _required_ - Your API Key available from your developer portal
* `sportIds` - _optional_ - A comma-separated list of sportsIds for which to retrieve topBets for
* `competitionIds` - _optional_ - A comma-separated list of competitionIds for which to retrieve topBets for
* `limit` - _optional_ - Specify the number of results to return
* `fields` - _optional_ - Specify an absolute field list to return (Comma-Separated List)
* `include` - _optional_ - Specify fields in addition to the default to return (Comma-Separated List)
* `exclude` - _optional_ - Specify fields from the default to exclude (Comma-Separated List)
* `param_topBetEventId` - _optional_ - The event ID to retrieve top bet information for. Multiple events up to 5 may be used
* `sortName` - _optional_ - The market sort code used to further filter event results. Please note this can only be used with event id(s).
* `culture` - _optional_ - Code used to return responses in language other than English, acceptable values are de-DE|es-ES|fr-FR|nn-NO|fi-FI|ru-RU|pt-PT|hu-HU|sl-SL|ga-IE|en-CA|sr-Latn|sv-SE|el=GR|zh-CHS|it-IT|zh-CHT|cs-CZ|de-AT|ja-JP|pl-PL|da-DK|ro-RO|nl-NL|tr-TR
* `Locale` - _optional_ - Code used to select a set of top bets settings, default is "whapi" which allows events set in far future to be included, setting the value to "en-GB" will activate english sportsbook settings, mirroring top bets on the website, which restricts events returned to those taking place in next 36 hours. Acceptable values (not all heve their own settings - if none currently available for that locale - en-GB will be used) are de-DE|whapi|en-GB|es-ES|fr-FR|nn-NO|fi-FI|ru-RU|pt-PT|hu-HU|sl-SL|ga-IE|en-CA|sr-Latn|sv-SE|el=GR|zh-CHS|it-IT|zh-CHT|cs-CZ|de-AT|ja-JP|pl-PL|da-DK|ro-RO|nl-NL|tr-TR

## License

**flow**ground :- Telekom iPaaS / whapi-com-sportsdata-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
