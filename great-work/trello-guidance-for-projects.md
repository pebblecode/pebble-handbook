# Trello Guidance for Projects

We use Trello pretty extensively and I’ve had a few people a bit confused about the best way to do this.

I’ll start off by saying you can use Trello boards for whatever you want, shared with whomever you want. For example,
I’ve seen some people using them like a distributed whiteboard with post it notes and it seem to be good for that. 

However, if you’re trying to use a Trello Board for running a project I think there are some steps you can take to 
make things more effective.

## Should I add a new board?

There is no hard and fast rules about when you should add a new board, however, I would recommend creating a new one 
for each project.
 
Projects have teams; you can add all the team members to the board. The team works on tasks; they will need to be able 
to edit their own cards. 

Projects should have few dependencies to tasks on other boards. If you have many tasks depending on other tasks then 
it is giving you a hint they should be merged. 

If you don't have a specific project, but still want to track some work, you should think about what the scope of the 
board (or project) should be. For example, we’ve made a distinction between developing the website and the content for 
the website, the reason is because they generally have different teams doing the work.

## How do I create a board?

When creating a board, for most projects its best to select the Team of pebble {code} and make the board Team Visible. 
Only people added to the board can edit it so you’ll need to add them individually. 

## What columns should I add to the board?

You should try to model your workflow, moving from left to right. At a minimum, I would recommend: Backlog, In Progress 
and Done. Work items (such as, user stories, bugs or tasks) should remain unassigned on the backlog until someone begins 
working on them. When someone begins working on the item, they should assign themselves and then when complete move to the 
done column.  

If you’re running Sprints you’ll likely need an extra column; Backlog, Current Sprint, In Progress and Done. 

Feel free to experiment by adding extra columns to the board. For example, I’ve seen teams replace Done with Reviewed, 
Tested and Deployed. 

By visualising your workflow, it means that it is easier to reason about and improve. For example, if you notice a lot of 
tickets getting stuck in a column, like Code Review, then it highlights that you need to put effort into removing that 
bottleneck.

Sometimes you’ll see a Kaizen column; this is just a place for capturing the notes from the meeting. Actions should be 
placed on the backlog like any other work item.

## My tasks seem to spend ages in, “In Progress”

If a task isn't in progress you can move it back home, but if someone has started work on it, then it should generally 
not go backwards. Instead, you should try to break down the ticket into the constituent tasks, moving the completed 
parts into done and the work outstanding into the backlog. 

Also consider only working on SMART tasks. Sometimes teams explicitly call out this break down process with a Ready 
column before in progress. The backlog items just represent things to be discussed at the next planning meeting.

## Should I track the same task on multiple boards? How do I manage dependencies?

Avoid having the same thing tracked more than once. Things need to be tracked somewhere, best to have it in one place. 

When you have a dependency, you should just use links from one ticket to another, but again, they should be avoided 
where possible. Consider using a Scrum of Scrum type meeting to disseminate this information.

## How do I manage re-occurring tasks?

I would recommend using your calendar and inviting the relevant people. Your calendar is a reliable way to track things. 
Schedule an appointment, you can put a link in your card if you want or vice versa. 

If the task is reoccurring a lot and has multiple stages you can consider either adding extra columns or modelling the 
process as another board. 

## We’ve got too many boards, how do I find my board?

Please take the time to delete/archive your board after your project finishes. We will do a periodic cleanup.
