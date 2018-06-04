Learning React using Tyler Mcginnis tutorial

React is a library for building user interfaces

Build a large app by compiling many small apps together

Composition:
```
<Container>
  <Navbar/>
  <Header/>
  <DatePicker/>
    <Calendar/>
  </DatePicker>
</Container>
```
You can ruse components on different pages e.g. on Twitter, who to follow on different pages

```javascript
// child function
function getProfilePic(username) {
  return 'https://photo.fb.com/' + username
}
// child function
function getProfileLink(username) {
  return 'https://fb.com/' + username
}
// parent function
function getAvatarInfo(username) {
  return{
    pic:getProfilePic(username)
    link:getProfileLink(username)
  }
}
// call parent function
get getAvatarInfo('alexmccarroll')
```

Unidirectional data flow:

Shared mutable state: sharing the same state throughout your application
