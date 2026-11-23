# HallRide: Campus Shuttle Information and Queue System

**Team:** Larp Squad  
**Document owner:** Moyo  
**Status:** Product requirements draft  
**Date:** 23 November 2026

## 1. Overview

HallRide is a proposed mobile-friendly service for sharing campus shuttle information and showing how many students are waiting at selected stops. Students could check the timetable and current trip status, then join a queue. Drivers or a transport coordinator would update departures, delays and cancellations. During the pilot, the coordinator—not the software—would make dispatch decisions.

The first pilot would focus on one route serving Samuel Akande Hall and a nearby destination, if campus transport staff approve the route. The team should choose the final route and stops after observing demand and speaking with students and operators. Other halls can be considered after the pilot.

## 2. Problem

The team’s initial problem is that students may have difficulty knowing when campus transport will arrive or whether it has room. Drivers and transport staff may not have a clear view of the number of students waiting at each stop. If this is confirmed, it can leave students unsure whether to wait, walk or find another option, while operators have little information to plan service.

This is a problem hypothesis, not a measured finding. No completed interviews, survey results, or stop counts were included in the material provided for this PRD. Before the pilot, Larp Squad should speak with students, drivers and the transport unit, and observe the proposed stops at the times students identify as busy. The research should establish how students get transport information today, how long they wait, how drivers receive dispatch instructions, and whether updated shuttle information would help.

The system cannot solve a shortage of vehicles by itself. If research shows that capacity is the main issue, HallRide may help document unmet demand, but the university would need to decide whether to change service levels.

## 3. Users

- **Students who use campus shuttles** need reliable information about routes, departures, delays and queues so they can decide where and when to wait.
- **Drivers** need a quick way to report a trip’s status and see the number of people waiting at upcoming stops.
- **The transport coordinator** needs to monitor the pilot route, keep information current and make dispatch decisions.

## 4. Goals and non-goals

### Goals

1. Make the pilot route and its stops easy for students to find.
2. Show the latest known departure and service status, including when it was last updated.
3. Give the coordinator a basic view of queue sizes at pilot stops.
4. Learn whether shared status and queue information is useful to students and manageable for drivers.
5. Collect enough pilot data to make an informed decision about continuing or changing the service.

### Not included in the pilot

- Automatic dispatch or route optimization.
- Continuous live GPS tracking.
- Payments, fares or a digital wallet.
- Night-ride or emergency-response promises.
- Campus-wide coverage, predictive analytics or a native mobile app.

These can be considered later if research, approvals and pilot results support them.

## 5. Proposed first version

HallRide will be a mobile-friendly web app for one approved route and a small pilot group. It will show the route, stops, planned departures and the latest status entered by a driver or coordinator. Students can join or leave a queue at a pilot stop and see their place in it. Drivers or the coordinator can mark a trip as boarding, departed, delayed, cancelled or complete. The coordinator can view queue counts and decide whether to contact a driver or adjust service.

The app should make clear that a queue position is not a guaranteed seat or exact arrival time. The displayed status must include the time of its last update; old information should be marked as unconfirmed.

## 6. Requirements

### Student features

- View the pilot route, stops and timetable.
- View the latest trip status and when it was updated.
- Join or leave the queue for an available stop.
- View queue position or the number of people ahead.
- Report a delay, incorrect status or other service issue.
- Access the timetable when the live status is unavailable.

### Driver and coordinator features

- Authorized users can update the trip status.
- Drivers can see the queue count at pilot stops.
- The coordinator can mark a trip delayed, cancelled or complete.
- The coordinator can view current queue counts by stop.
- The system records queue and status changes for pilot review.

### Operating rules

- Queueing does not guarantee a seat; vehicle capacity and driver instructions take precedence.
- A student can have one active queue entry at a time.
- Dispatch decisions remain with the transport coordinator.
- Drivers must not be expected to use the app while driving.
- Only information needed to operate and evaluate the pilot should be collected. Access and deletion periods must be agreed before launch.

## 7. Success measures

The team should record a baseline at the selected stop before the pilot. The pilot will compare:

- Student wait times before and during the pilot.
- Whether the app’s status matches actual departures, delays and cancellations.
- How often students use the queue and whether they find it useful.
- Whether drivers and the coordinator can keep information current without disrupting their work.
- Student feedback about clarity, trust and usefulness.

The team should report the measured results, including cases where wait times did not improve. The app should not be credited for changes caused by additional vehicles, schedule changes or other factors without noting those changes.

## 8. Pilot plan

1. **Research:** Interview students who use the proposed route, speak with drivers and the transport coordinator, and observe the stops during busy periods identified by students.
2. **Confirm scope:** Select one route and its stops based on the research. Confirm operating hours, capacity, permissions and who will update trip status.
3. **Small trial:** Test the timetable, queue and status updates with a small group and participating drivers.
4. **Review:** Compare pilot results with the baseline and gather feedback from students, drivers and the coordinator.
5. **Decision:** Continue, revise or stop the pilot based on usefulness, status accuracy, staff effort and university approval. Expand to more halls only after the first route works operationally.

## 9. Risks and constraints

| Risk | Response |
|---|---|
| There are not enough vehicles to meet demand. | Explain that the service shares information but does not add capacity; record unmet demand for the transport unit. |
| Drivers cannot update the app regularly. | Agree on a simple process with drivers before launch and allow coordinator updates. Never require updates while driving. |
| Students rely on an outdated status. | Show the last update time and mark old status as unconfirmed. |
| Students do not trust the queue order. | Explain the boarding rules and review complaints during the trial. |
| Internet access is unreliable. | Keep the timetable accessible when live status is unavailable. |
| Student activity data is exposed or retained unnecessarily. | Minimize collection, restrict access and agree on a deletion schedule before the pilot. |
| The university does not approve the pilot. | Treat approval and driver participation as prerequisites; do not launch without them. |

## 10. Dependencies and open questions

The pilot needs approval from the university or transport unit, a participating driver, an agreed route and stops, and a named coordinator responsible for keeping service information current. The team must confirm how students will be verified, what data can be collected, and who will handle complaints.

Before implementation, the team must also establish actual operating hours, vehicle capacity, departure patterns and the current dispatch process. The programming language and technical design should be chosen after these needs and constraints are understood.

