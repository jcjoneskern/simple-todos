Built with React and Meteor.

Following along with https://www.meteor.com/tutorials/react/creating-an-app

------

The test in the tutorial doesn't seem to work. Following the tutorial as is gives the failure:
`Error: Meteor.userId can only be invoked in method calls or publications.`

Some googling implies that the fix is to change
`if (task.owner !== Meteor.userId())`
to
`if (task.owner !== this.userId())`
but then error message says `this.userId() is not a function`

At least the app itself works?
