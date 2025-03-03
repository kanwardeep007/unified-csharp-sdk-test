# Calendar
(*Calendar*)

## Overview

### Available Operations

* [CreateCalendarCalendar](#createcalendarcalendar) - Create a calendar
* [CreateCalendarEvent](#createcalendarevent) - Create an event
* [CreateCalendarLink](#createcalendarlink) - Create a link
* [GetCalendarCalendar](#getcalendarcalendar) - Retrieve a calendar
* [GetCalendarEvent](#getcalendarevent) - Retrieve an event
* [GetCalendarLink](#getcalendarlink) - Retrieve a link
* [GetCalendarRecording](#getcalendarrecording) - Retrieve a recording
* [ListCalendarBusies](#listcalendarbusies) - List all busies
* [ListCalendarCalendars](#listcalendarcalendars) - List all calendars
* [ListCalendarEvents](#listcalendarevents) - List all events
* [ListCalendarLinks](#listcalendarlinks) - List all links
* [ListCalendarRecordings](#listcalendarrecordings) - List all recordings
* [PatchCalendarCalendar](#patchcalendarcalendar) - Update a calendar
* [PatchCalendarEvent](#patchcalendarevent) - Update an event
* [PatchCalendarLink](#patchcalendarlink) - Update a link
* [RemoveCalendarCalendar](#removecalendarcalendar) - Remove a calendar
* [RemoveCalendarEvent](#removecalendarevent) - Remove an event
* [RemoveCalendarLink](#removecalendarlink) - Remove a link
* [UpdateCalendarCalendar](#updatecalendarcalendar) - Update a calendar
* [UpdateCalendarEvent](#updatecalendarevent) - Update an event
* [UpdateCalendarLink](#updatecalendarlink) - Update a link

## CreateCalendarCalendar

Create a calendar

### Example Usage

```csharp
using System.Collections.Generic;
using UnifiedTo;
using UnifiedTo.Models.Components;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

var res = await sdk.Calendar.CreateCalendarCalendarAsync(
    calendarCalendar: new CalendarCalendar() {
        Name = "<value>",
    },
    connectionId: "<id>",
    fields: new List<string>() {
        "<value>",
    }
);

// handle response
```

### Parameters

| Parameter                                                       | Type                                                            | Required                                                        | Description                                                     |
| --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- |
| `CalendarCalendar`                                              | [CalendarCalendar](../../Models/Components/CalendarCalendar.md) | :heavy_check_mark:                                              | N/A                                                             |
| `ConnectionId`                                                  | *string*                                                        | :heavy_check_mark:                                              | ID of the connection                                            |
| `Fields`                                                        | List<*string*>                                                  | :heavy_minus_sign:                                              | Comma-delimited fields to return                                |

### Response

**[CreateCalendarCalendarResponse](../../Models/Requests/CreateCalendarCalendarResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |

## CreateCalendarEvent

Create an event

### Example Usage

```csharp
using System.Collections.Generic;
using UnifiedTo;
using UnifiedTo.Models.Components;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

var res = await sdk.Calendar.CreateCalendarEventAsync(
    calendarEvent: new CalendarEvent() {
        EndAt = "<value>",
        StartAt = "<value>",
        Subject = "<value>",
    },
    connectionId: "<id>",
    fields: new List<string>() {
        "<value>",
    }
);

// handle response
```

### Parameters

| Parameter                                                 | Type                                                      | Required                                                  | Description                                               |
| --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- |
| `CalendarEvent`                                           | [CalendarEvent](../../Models/Components/CalendarEvent.md) | :heavy_check_mark:                                        | N/A                                                       |
| `ConnectionId`                                            | *string*                                                  | :heavy_check_mark:                                        | ID of the connection                                      |
| `Fields`                                                  | List<*string*>                                            | :heavy_minus_sign:                                        | Comma-delimited fields to return                          |

### Response

**[CreateCalendarEventResponse](../../Models/Requests/CreateCalendarEventResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |

## CreateCalendarLink

Create a link

### Example Usage

```csharp
using System.Collections.Generic;
using UnifiedTo;
using UnifiedTo.Models.Components;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

var res = await sdk.Calendar.CreateCalendarLinkAsync(
    calendarLink: new CalendarLink() {
        Url = "https://sturdy-begonia.biz/",
    },
    connectionId: "<id>",
    fields: new List<string>() {
        "<value>",
    }
);

// handle response
```

### Parameters

| Parameter                                               | Type                                                    | Required                                                | Description                                             |
| ------------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------------------- |
| `CalendarLink`                                          | [CalendarLink](../../Models/Components/CalendarLink.md) | :heavy_check_mark:                                      | N/A                                                     |
| `ConnectionId`                                          | *string*                                                | :heavy_check_mark:                                      | ID of the connection                                    |
| `Fields`                                                | List<*string*>                                          | :heavy_minus_sign:                                      | Comma-delimited fields to return                        |

### Response

**[CreateCalendarLinkResponse](../../Models/Requests/CreateCalendarLinkResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |

## GetCalendarCalendar

Retrieve a calendar

### Example Usage

```csharp
using System.Collections.Generic;
using UnifiedTo;
using UnifiedTo.Models.Components;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

var res = await sdk.Calendar.GetCalendarCalendarAsync(
    connectionId: "<id>",
    id: "<id>",
    fields: new List<string>() {
        "<value>",
    }
);

// handle response
```

### Parameters

| Parameter                        | Type                             | Required                         | Description                      |
| -------------------------------- | -------------------------------- | -------------------------------- | -------------------------------- |
| `ConnectionId`                   | *string*                         | :heavy_check_mark:               | ID of the connection             |
| `Id`                             | *string*                         | :heavy_check_mark:               | ID of the Calendar               |
| `Fields`                         | List<*string*>                   | :heavy_minus_sign:               | Comma-delimited fields to return |

### Response

**[GetCalendarCalendarResponse](../../Models/Requests/GetCalendarCalendarResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |

## GetCalendarEvent

Retrieve an event

### Example Usage

```csharp
using System.Collections.Generic;
using UnifiedTo;
using UnifiedTo.Models.Components;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

var res = await sdk.Calendar.GetCalendarEventAsync(
    connectionId: "<id>",
    id: "<id>",
    fields: new List<string>() {
        "<value>",
    }
);

// handle response
```

### Parameters

| Parameter                        | Type                             | Required                         | Description                      |
| -------------------------------- | -------------------------------- | -------------------------------- | -------------------------------- |
| `ConnectionId`                   | *string*                         | :heavy_check_mark:               | ID of the connection             |
| `Id`                             | *string*                         | :heavy_check_mark:               | ID of the Event                  |
| `Fields`                         | List<*string*>                   | :heavy_minus_sign:               | Comma-delimited fields to return |

### Response

**[GetCalendarEventResponse](../../Models/Requests/GetCalendarEventResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |

## GetCalendarLink

Retrieve a link

### Example Usage

```csharp
using System.Collections.Generic;
using UnifiedTo;
using UnifiedTo.Models.Components;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

var res = await sdk.Calendar.GetCalendarLinkAsync(
    connectionId: "<id>",
    id: "<id>",
    fields: new List<string>() {
        "<value>",
    }
);

// handle response
```

### Parameters

| Parameter                        | Type                             | Required                         | Description                      |
| -------------------------------- | -------------------------------- | -------------------------------- | -------------------------------- |
| `ConnectionId`                   | *string*                         | :heavy_check_mark:               | ID of the connection             |
| `Id`                             | *string*                         | :heavy_check_mark:               | ID of the Link                   |
| `Fields`                         | List<*string*>                   | :heavy_minus_sign:               | Comma-delimited fields to return |

### Response

**[GetCalendarLinkResponse](../../Models/Requests/GetCalendarLinkResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |

## GetCalendarRecording

Retrieve a recording

### Example Usage

```csharp
using System.Collections.Generic;
using UnifiedTo;
using UnifiedTo.Models.Components;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

var res = await sdk.Calendar.GetCalendarRecordingAsync(
    connectionId: "<id>",
    id: "<id>",
    fields: new List<string>() {
        "<value>",
    }
);

// handle response
```

### Parameters

| Parameter                        | Type                             | Required                         | Description                      |
| -------------------------------- | -------------------------------- | -------------------------------- | -------------------------------- |
| `ConnectionId`                   | *string*                         | :heavy_check_mark:               | ID of the connection             |
| `Id`                             | *string*                         | :heavy_check_mark:               | ID of the Recording              |
| `Fields`                         | List<*string*>                   | :heavy_minus_sign:               | Comma-delimited fields to return |

### Response

**[GetCalendarRecordingResponse](../../Models/Requests/GetCalendarRecordingResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |

## ListCalendarBusies

List all busies

### Example Usage

```csharp
using UnifiedTo;
using UnifiedTo.Models.Components;
using UnifiedTo.Models.Requests;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

ListCalendarBusiesRequest req = new ListCalendarBusiesRequest() {
    ConnectionId = "<id>",
};

var res = await sdk.Calendar.ListCalendarBusiesAsync(req);

// handle response
```

### Parameters

| Parameter                                                                       | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `request`                                                                       | [ListCalendarBusiesRequest](../../Models/Requests/ListCalendarBusiesRequest.md) | :heavy_check_mark:                                                              | The request object to use for the request.                                      |

### Response

**[ListCalendarBusiesResponse](../../Models/Requests/ListCalendarBusiesResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |

## ListCalendarCalendars

List all calendars

### Example Usage

```csharp
using UnifiedTo;
using UnifiedTo.Models.Components;
using UnifiedTo.Models.Requests;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

ListCalendarCalendarsRequest req = new ListCalendarCalendarsRequest() {
    ConnectionId = "<id>",
};

var res = await sdk.Calendar.ListCalendarCalendarsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                             | Type                                                                                  | Required                                                                              | Description                                                                           |
| ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------- |
| `request`                                                                             | [ListCalendarCalendarsRequest](../../Models/Requests/ListCalendarCalendarsRequest.md) | :heavy_check_mark:                                                                    | The request object to use for the request.                                            |

### Response

**[ListCalendarCalendarsResponse](../../Models/Requests/ListCalendarCalendarsResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |

## ListCalendarEvents

List all events

### Example Usage

```csharp
using UnifiedTo;
using UnifiedTo.Models.Components;
using UnifiedTo.Models.Requests;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

ListCalendarEventsRequest req = new ListCalendarEventsRequest() {
    ConnectionId = "<id>",
};

var res = await sdk.Calendar.ListCalendarEventsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                       | Type                                                                            | Required                                                                        | Description                                                                     |
| ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| `request`                                                                       | [ListCalendarEventsRequest](../../Models/Requests/ListCalendarEventsRequest.md) | :heavy_check_mark:                                                              | The request object to use for the request.                                      |

### Response

**[ListCalendarEventsResponse](../../Models/Requests/ListCalendarEventsResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |

## ListCalendarLinks

List all links

### Example Usage

```csharp
using UnifiedTo;
using UnifiedTo.Models.Components;
using UnifiedTo.Models.Requests;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

ListCalendarLinksRequest req = new ListCalendarLinksRequest() {
    ConnectionId = "<id>",
};

var res = await sdk.Calendar.ListCalendarLinksAsync(req);

// handle response
```

### Parameters

| Parameter                                                                     | Type                                                                          | Required                                                                      | Description                                                                   |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------- |
| `request`                                                                     | [ListCalendarLinksRequest](../../Models/Requests/ListCalendarLinksRequest.md) | :heavy_check_mark:                                                            | The request object to use for the request.                                    |

### Response

**[ListCalendarLinksResponse](../../Models/Requests/ListCalendarLinksResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |

## ListCalendarRecordings

List all recordings

### Example Usage

```csharp
using UnifiedTo;
using UnifiedTo.Models.Components;
using UnifiedTo.Models.Requests;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

ListCalendarRecordingsRequest req = new ListCalendarRecordingsRequest() {
    ConnectionId = "<id>",
};

var res = await sdk.Calendar.ListCalendarRecordingsAsync(req);

// handle response
```

### Parameters

| Parameter                                                                               | Type                                                                                    | Required                                                                                | Description                                                                             |
| --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| `request`                                                                               | [ListCalendarRecordingsRequest](../../Models/Requests/ListCalendarRecordingsRequest.md) | :heavy_check_mark:                                                                      | The request object to use for the request.                                              |

### Response

**[ListCalendarRecordingsResponse](../../Models/Requests/ListCalendarRecordingsResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |

## PatchCalendarCalendar

Update a calendar

### Example Usage

```csharp
using System.Collections.Generic;
using UnifiedTo;
using UnifiedTo.Models.Components;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

var res = await sdk.Calendar.PatchCalendarCalendarAsync(
    calendarCalendar: new CalendarCalendar() {
        Name = "<value>",
    },
    connectionId: "<id>",
    id: "<id>",
    fields: new List<string>() {
        "<value>",
    }
);

// handle response
```

### Parameters

| Parameter                                                       | Type                                                            | Required                                                        | Description                                                     |
| --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- |
| `CalendarCalendar`                                              | [CalendarCalendar](../../Models/Components/CalendarCalendar.md) | :heavy_check_mark:                                              | N/A                                                             |
| `ConnectionId`                                                  | *string*                                                        | :heavy_check_mark:                                              | ID of the connection                                            |
| `Id`                                                            | *string*                                                        | :heavy_check_mark:                                              | ID of the Calendar                                              |
| `Fields`                                                        | List<*string*>                                                  | :heavy_minus_sign:                                              | Comma-delimited fields to return                                |

### Response

**[PatchCalendarCalendarResponse](../../Models/Requests/PatchCalendarCalendarResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |

## PatchCalendarEvent

Update an event

### Example Usage

```csharp
using System.Collections.Generic;
using UnifiedTo;
using UnifiedTo.Models.Components;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

var res = await sdk.Calendar.PatchCalendarEventAsync(
    calendarEvent: new CalendarEvent() {
        EndAt = "<value>",
        StartAt = "<value>",
        Subject = "<value>",
    },
    connectionId: "<id>",
    id: "<id>",
    fields: new List<string>() {
        "<value>",
    }
);

// handle response
```

### Parameters

| Parameter                                                 | Type                                                      | Required                                                  | Description                                               |
| --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- |
| `CalendarEvent`                                           | [CalendarEvent](../../Models/Components/CalendarEvent.md) | :heavy_check_mark:                                        | N/A                                                       |
| `ConnectionId`                                            | *string*                                                  | :heavy_check_mark:                                        | ID of the connection                                      |
| `Id`                                                      | *string*                                                  | :heavy_check_mark:                                        | ID of the Event                                           |
| `Fields`                                                  | List<*string*>                                            | :heavy_minus_sign:                                        | Comma-delimited fields to return                          |

### Response

**[PatchCalendarEventResponse](../../Models/Requests/PatchCalendarEventResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |

## PatchCalendarLink

Update a link

### Example Usage

```csharp
using System.Collections.Generic;
using UnifiedTo;
using UnifiedTo.Models.Components;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

var res = await sdk.Calendar.PatchCalendarLinkAsync(
    calendarLink: new CalendarLink() {
        Url = "https://curly-skyline.biz/",
    },
    connectionId: "<id>",
    id: "<id>",
    fields: new List<string>() {
        "<value>",
    }
);

// handle response
```

### Parameters

| Parameter                                               | Type                                                    | Required                                                | Description                                             |
| ------------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------------------- |
| `CalendarLink`                                          | [CalendarLink](../../Models/Components/CalendarLink.md) | :heavy_check_mark:                                      | N/A                                                     |
| `ConnectionId`                                          | *string*                                                | :heavy_check_mark:                                      | ID of the connection                                    |
| `Id`                                                    | *string*                                                | :heavy_check_mark:                                      | ID of the Link                                          |
| `Fields`                                                | List<*string*>                                          | :heavy_minus_sign:                                      | Comma-delimited fields to return                        |

### Response

**[PatchCalendarLinkResponse](../../Models/Requests/PatchCalendarLinkResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |

## RemoveCalendarCalendar

Remove a calendar

### Example Usage

```csharp
using UnifiedTo;
using UnifiedTo.Models.Components;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

var res = await sdk.Calendar.RemoveCalendarCalendarAsync(
    connectionId: "<id>",
    id: "<id>"
);

// handle response
```

### Parameters

| Parameter            | Type                 | Required             | Description          |
| -------------------- | -------------------- | -------------------- | -------------------- |
| `ConnectionId`       | *string*             | :heavy_check_mark:   | ID of the connection |
| `Id`                 | *string*             | :heavy_check_mark:   | ID of the Calendar   |

### Response

**[RemoveCalendarCalendarResponse](../../Models/Requests/RemoveCalendarCalendarResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |

## RemoveCalendarEvent

Remove an event

### Example Usage

```csharp
using UnifiedTo;
using UnifiedTo.Models.Components;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

var res = await sdk.Calendar.RemoveCalendarEventAsync(
    connectionId: "<id>",
    id: "<id>"
);

// handle response
```

### Parameters

| Parameter            | Type                 | Required             | Description          |
| -------------------- | -------------------- | -------------------- | -------------------- |
| `ConnectionId`       | *string*             | :heavy_check_mark:   | ID of the connection |
| `Id`                 | *string*             | :heavy_check_mark:   | ID of the Event      |

### Response

**[RemoveCalendarEventResponse](../../Models/Requests/RemoveCalendarEventResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |

## RemoveCalendarLink

Remove a link

### Example Usage

```csharp
using UnifiedTo;
using UnifiedTo.Models.Components;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

var res = await sdk.Calendar.RemoveCalendarLinkAsync(
    connectionId: "<id>",
    id: "<id>"
);

// handle response
```

### Parameters

| Parameter            | Type                 | Required             | Description          |
| -------------------- | -------------------- | -------------------- | -------------------- |
| `ConnectionId`       | *string*             | :heavy_check_mark:   | ID of the connection |
| `Id`                 | *string*             | :heavy_check_mark:   | ID of the Link       |

### Response

**[RemoveCalendarLinkResponse](../../Models/Requests/RemoveCalendarLinkResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |

## UpdateCalendarCalendar

Update a calendar

### Example Usage

```csharp
using System.Collections.Generic;
using UnifiedTo;
using UnifiedTo.Models.Components;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

var res = await sdk.Calendar.UpdateCalendarCalendarAsync(
    calendarCalendar: new CalendarCalendar() {
        Name = "<value>",
    },
    connectionId: "<id>",
    id: "<id>",
    fields: new List<string>() {
        "<value>",
    }
);

// handle response
```

### Parameters

| Parameter                                                       | Type                                                            | Required                                                        | Description                                                     |
| --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- | --------------------------------------------------------------- |
| `CalendarCalendar`                                              | [CalendarCalendar](../../Models/Components/CalendarCalendar.md) | :heavy_check_mark:                                              | N/A                                                             |
| `ConnectionId`                                                  | *string*                                                        | :heavy_check_mark:                                              | ID of the connection                                            |
| `Id`                                                            | *string*                                                        | :heavy_check_mark:                                              | ID of the Calendar                                              |
| `Fields`                                                        | List<*string*>                                                  | :heavy_minus_sign:                                              | Comma-delimited fields to return                                |

### Response

**[UpdateCalendarCalendarResponse](../../Models/Requests/UpdateCalendarCalendarResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |

## UpdateCalendarEvent

Update an event

### Example Usage

```csharp
using System.Collections.Generic;
using UnifiedTo;
using UnifiedTo.Models.Components;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

var res = await sdk.Calendar.UpdateCalendarEventAsync(
    calendarEvent: new CalendarEvent() {
        EndAt = "<value>",
        StartAt = "<value>",
        Subject = "<value>",
    },
    connectionId: "<id>",
    id: "<id>",
    fields: new List<string>() {
        "<value>",
    }
);

// handle response
```

### Parameters

| Parameter                                                 | Type                                                      | Required                                                  | Description                                               |
| --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- | --------------------------------------------------------- |
| `CalendarEvent`                                           | [CalendarEvent](../../Models/Components/CalendarEvent.md) | :heavy_check_mark:                                        | N/A                                                       |
| `ConnectionId`                                            | *string*                                                  | :heavy_check_mark:                                        | ID of the connection                                      |
| `Id`                                                      | *string*                                                  | :heavy_check_mark:                                        | ID of the Event                                           |
| `Fields`                                                  | List<*string*>                                            | :heavy_minus_sign:                                        | Comma-delimited fields to return                          |

### Response

**[UpdateCalendarEventResponse](../../Models/Requests/UpdateCalendarEventResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |

## UpdateCalendarLink

Update a link

### Example Usage

```csharp
using System.Collections.Generic;
using UnifiedTo;
using UnifiedTo.Models.Components;

var sdk = new UnifiedToSDK(security: new Security() {
    Jwt = "<YOUR_API_KEY_HERE>",
});

var res = await sdk.Calendar.UpdateCalendarLinkAsync(
    calendarLink: new CalendarLink() {
        Url = "https://quiet-coordination.name",
    },
    connectionId: "<id>",
    id: "<id>",
    fields: new List<string>() {
        "<value>",
    }
);

// handle response
```

### Parameters

| Parameter                                               | Type                                                    | Required                                                | Description                                             |
| ------------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------------------- | ------------------------------------------------------- |
| `CalendarLink`                                          | [CalendarLink](../../Models/Components/CalendarLink.md) | :heavy_check_mark:                                      | N/A                                                     |
| `ConnectionId`                                          | *string*                                                | :heavy_check_mark:                                      | ID of the connection                                    |
| `Id`                                                    | *string*                                                | :heavy_check_mark:                                      | ID of the Link                                          |
| `Fields`                                                | List<*string*>                                          | :heavy_minus_sign:                                      | Comma-delimited fields to return                        |

### Response

**[UpdateCalendarLinkResponse](../../Models/Requests/UpdateCalendarLinkResponse.md)**

### Errors

| Error Type                           | Status Code                          | Content Type                         |
| ------------------------------------ | ------------------------------------ | ------------------------------------ |
| UnifiedTo.Models.Errors.SDKException | 4XX, 5XX                             | \*/\*                                |