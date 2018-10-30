# VueJs communication between components

## Component
    - has a built in enviromment
    - ideally, does not know about other components
    - controls only what is indise it

## User Interface
    - is made up of components
    - arranged in mainly 3 different ways
      and hence communicates ...
    - parent has child(ren)
    - child has (one) parent
    - siblings or unrelated components - at any level

## Communication between components
    - let it know to look for changed situation
    - can make a change by sending data

## Direct communication - downward
    - parent can directly affect child data
    - use props to pass data

## Direct communication - upward - to parent
    - child can 'tell' the parent about 'something'
    - use an 'event' to let the parent know

## Long distance communication - to any other component
    - any component to any other component
    - use an 'event bus'

## Communicating in the blind - to anyone - using vuex 'store'
    - to whomever it may concern
    - any component can access the change
    - it only needs to know the name(s) of the store.state varibles
        to track it
    - the change is propagated reactively
    - best suited for larger application, because of extra code

Jay Kelkar (jkelkar at gmail.com)