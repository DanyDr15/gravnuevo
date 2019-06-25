---
title: ELEVADOR
---

<!-- # BIENVENIDOS
## Graficación y animación  -->
###Elevador

NIVEL 1
{
init: function(elevators, floors) {
var elevator = elevators[0]; // Let's use the first elevator

// Whenever the elevator is idle (has no more queued destinations) ...
elevator.on("idle", function() {
// let's go to all the floors (or did we forget one?)
elevator.goToFloor(0);
elevator.goToFloor(1);
});
},
update: function(dt, elevators, floors) {
// We normally don't need to do anything here
}
}

NIVEL 2
{
init: function(elevators, floors) {
var elevator = elevators[0]; // Let's use the first elevator

// Whenever the elevator is idle (has no more queued destinations) ...
elevator.on("idle", function() {
// let's go to all the floors (or did we forget one?)
var i;
for(i=0;i<=4;i++)
{

	elevator.goToFloor(i);   
}
});
},
update: function(dt, elevators, floors) {
// We normally don't need to do anything here
}
}

NIVEL 3
{
init: function(elevators, floors) {
var elevator = elevators[0]; // Let's use the first elevator

// Whenever the elevator is idle (has no more queued destinations) ...
elevator.on("idle", function() {
// let's go to all the floors (or did we forget one?)
var i;
for(i=0;i<=4;i++)
	{

		elevator.goToFloor(i);   
	}
;
for(i=4;i>=0;i--)
{

	elevator.goToFloor(i);   
}
});
},
update: function(dt, elevators, floors) {
// We normally don't need to do anything here
}
}

NIVEL 4
{
    init: function(elevators, floors) {
        var elevator = elevators[0]; // Let's use the first elevator
        var elevator1 = elevators[1]; // Let's use the first elevator

        // Whenever the elevator is idle (has no more queued destinations) ...
        elevator.on("idle", function() {
			// let's go to all the floors (or did we forget one?
			
            elevator.on("floor_button_pressed", function(floorNum) {// Es la funcion que se dispara cuando un pasajero ha presionado un botón dentro del ascensor.	

                // Maybe tell the elevator to go to that floor?
                elevator.goToFloor(floorNum); //y con este llamamos para que el ascesor vaya al piso que el usuario presiono
            })
            elevator1.on("floor_button_pressed", function(floorNum) {
                // Maybe tell the elevator to go to that floor?
                elevator1.goToFloor(floorNum);
            })
        });
    },
        update: function(dt, elevators, floors) {
            // We normally don't need to do anything here
        }
}

NIVEL 5
{
    init: function(elevators, floors) {
        var elevator = elevators[0]; // Let's use the first elevator
        var elevator1 = elevators[1]; // Let's use the first elevator
        var elevator2 = elevators[2]; // Let's use the first elevator
        var elevator3 = elevators[3]; // Let's use the first elevator

        // Whenever the elevator is idle (has no more queued destinations) ...
        elevator.on("idle", function() {
            // let's go to all the floors (or did we forget one?)
        /*  for(var i=0;i<=8;i++)
              {
                  elevator.goToFloor(i);
                  elevator1.goToFloor(i);

              }
         */
            elevator.on("floor_button_pressed", function(floorNum) {  // Es la funcion que se dispara cuando un pasajero ha presionado un botón dentro del ascensor.	 En este caso son 3 elevadores y utuilizamos la misma funcion para los 4
                // Maybe tell the elevator to go to that floor?
                elevator.goToFloor(floorNum);
            })
            elevator1.on("floor_button_pressed", function(floorNum) {
                // Maybe tell the elevator to go to that floor?
                elevator1.goToFloor(floorNum);
            })
            elevator2.on("floor_button_pressed", function(floorNum) {
                // Maybe tell the elevator to go to that floor?
                elevator2.goToFloor(floorNum);
            })
            elevator3.on("floor_button_pressed", function(floorNum) {
                // Maybe tell the elevator to go to that floor?
                elevator3.goToFloor(floorNum);
            }) 
        });
    },
        update: function(dt, elevators, floors) {
            // We normally don't need to do anything here
        }
}

NIVEL 6
{
    init: function(elevators, floors) {
        var elevator = elevators[0]; // Let's use the first elevator
        var elevator1 = elevators[1]; // Let's use the first elevator
        var elevator2 = elevators[2]; // Let's use the first elevator
        var elevator3 = elevators[3]; // Let's use the first elevator

        // Whenever the elevator is idle (has no more queued destinations) ...
        elevator.on("idle", function() {
            // let's go to all the floors (or did we forget one?)
        /*  for(var i=0;i<=8;i++)
              {
                  elevator.goToFloor(i);
                  elevator1.goToFloor(i);

              }
         */
            elevator.on("floor_button_pressed", function(floorNum) {// Es la funcion que se dispara cuando un pasajero ha presionado un botón dentro del ascensor.	 En este caso son 2 elevadores y utulizamos la misma funcion para los 2
                // Maybe tell the elevator to go to that floor?
                elevator.goToFloor(floorNum);
            })
            

            elevator1.on("floor_button_pressed", function(floorNum) {
                // Maybe tell the elevator to go to that floor?
                elevator1.goToFloor(floorNum);
            })            
        });
    },
        update: function(dt, elevators, floors) {
            // We normally don't need to do anything here
        }
}

NIVEL 7
{
    init: function(elevators, floors) {
        var elevator = elevators[0]; // Let's use the first elevator
        var elevator1 = elevators[1]; // Let's use the first elevator
        var elevator2 = elevators[2]; // Let's use the first elevator
        // Whenever the elevator is idle (has no more queued destinations) ...
        elevator.on("idle", function() {
            // let's go to all the floors (or did we forget one?)
        /*  for(var i=0;i<=8;i++)
              {
                  elevator.goToFloor(i);
                  elevator1.goToFloor(i);

              }
         */
            elevator.on("floor_button_pressed", function(floorNum) {
                // Maybe tell the elevator to go to that floor?
                elevator.goToFloor(floorNum);
            })
            elevator1.on("floor_button_pressed", function(floorNum) {
                // Maybe tell the elevator to go to that floor?
                elevator1.goToFloor(floorNum);
            })
            elevator2.on("floor_button_pressed", function(floorNum) {
                // Maybe tell the elevator to go to that floor?
                elevator2.goToFloor(floorNum);
            })
        });
    },
        update: function(dt, elevators, floors) {
            // We normally don't need to do anything here
        }
}

NIVEL 8 al 9
  {
    init: function(elevators, floors) {
        elevators.forEach(function(elevator, index) {
            elevator.on("floor_button_pressed", function(floorNum) {
                if (elevator.destinationQueue.indexOf(floorNum) == -1) { elevator.goToFloor(floorNum); }
            });
            elevator.on("passing_floor", function(floorNum, direction) {
                // Pick up passengers on the floor if there is room
                if (elevator.loadFactor() <= 0.7) {
                    if (direction == "up" && floors[floorNum].requestedUp) { elevator.goToFloor(floorNum, true); }
                    if (direction == "down" && floors[floorNum].requestedDown) { elevator.goToFloor(floorNum, true); }
                }
                // Stop at the floor first if it is in the queue
                if (elevator.destinationQueue.indexOf(floorNum) != -1) { 
                    elevator.destinationQueue.splice(elevator.destinationQueue.indexOf(floorNum), 1);
                    elevator.goToFloor(floorNum, true); 
                }
            });
            elevator.on("stopped_at_floor", function(floorNum) {
                if (elevator.destinationDirection() == "up") {
                    floors[floorNum].requestedUp = false;
                } else {
                    floors[floorNum].requestedDown = false;
                }
            });

            elevator.on("idle", function() {
                var requestedFloors = floors.filter(function(f) { return f.requestedUp || f.requestedDown; });
                var distances = requestedFloors.map(function(f) { return Math.abs(f.floorNum() - elevator.currentFloor()); });
                var floorIndex = Math.min.apply(null, distances);
                if (requestedFloors[floorIndex]) {
                    var floorNum = requestedFloors[floorIndex].floorNum();

                    floors[floorNum].requestedUp = false;
                    floors[floorNum].requestedDown = false;
                    elevator.goToFloor(floorNum);
                } else {
                    elevator.goToFloor(0);
                }
            })
        });

        floors.forEach(function(floor, index) {
            floor.requestedUp = false;
            floor.requestedDown = false;
            floor.on("up_button_pressed", function() {
                floor.requestedUp = true;
            });
            floor.on("down_button_pressed", function() {
                floor.requestedDown = true;
            });
        });
    },
        update: function(dt, elevators, floors) {
            // We normally don't need to do anything here
        }
}

NIVEL 10 al 11
{

  init: function(elevators, floors) {
    var getIdleElevator = function(floorNum, direction){
      console.log('Looking for elevator from', floorNum, direction, 'from', elevators.map(function(elevator){ return elevator.description() }));
      var floorMatch = elevators
      .filter(function(elevator){ return elevator.destination === floorNum && elevator.direction === direction})
      .pop();
      if (floorMatch) {
        console.log('Found elevator with directly matched floor and direction:', floorMatch.description());
        return null; // caller will be all good, elevator comming anyway;
      };
      var passThrough = elevators
      .filter(function(elevator){
        if (direction === 'up') {
          return elevator.destination > floorNum && elevator.currentFloor() < floorNum;
        } else if (direction === 'down') {
          return elevator.destination < floorNum && elevator.currentFloor() > floorNum;
        } else {
          return false;
        }
      })
      .pop()
      if (passThrough) {
        console.log('Found elevator with on the way:', passThrough.description());
        return null; // caller will be all good, elevator comming anyway;
      };
      console.log('Fallback to finding closest');
      return elevators
        .filter(function(elevator) { return elevator.isIdle() })
        .sort(function(a, b){ return Math.abs(b - floorNum) - Math.abs(a - floorNum)})
        .pop();
    };
    var getBusyFloor = function(floorNum) {
      var isBusy = function(floor){
        return floor.buttonStates.up === 'activated' || floor.buttonStates.down === 'activated'
      };
      if (isBusy(floors[floorNum])) {
        return floors[floorNum];
      };



      return floors
        .filter(isBusy)
        .sort(function(a, b){ return Math.abs(b.floorNum() - floorNum) - Math.abs(a.floorNum() - floorNum)})
        .pop();
    }
    var isFloorRequestedOutside = function(floorNum, direction) { return floors[floorNum].buttonStates[direction] === 'activated'; }
    var i = 0;
    elevators.forEach(function(elevator) {
      elevator.number = i++;
      elevator.destination = null;
      elevator.direction = null;
      elevator.description = function() { return "elevator-" +
        elevator.number +
        (elevator.destination !== null ? '->' + elevator.destination : '') +
        (elevator.direction ? '-' + elevator.direction : '')}
      elevator.isIdle = function() { return !elevator.destination };
      elevator.isFloorRequestedInside = function(floorNum) { return elevator.getPressedFloors().indexOf(floorNum) > 0 };
      elevator.switchLights = function(direction) {
        if (direction === 'up') {
          elevator.goingUpIndicator(true);
          elevator.goingDownIndicator(false);
        } else if (direction === 'down') {
          elevator.goingDownIndicator(true);
          elevator.goingUpIndicator(false);
        } else {
          elevator.goingUpIndicator(true);
          elevator.goingDownIndicator(true);
        }
      }
      elevator.navigateTo = function(floorNum, direction) {
        if (elevator.destination !== null) {
          console.log(elevator.description(), 'Attempted to reschedule running elevator, X_X');
          return;
        }
        elevator.destination = floorNum;
        elevator.direction = direction;
        console.log(elevator.description(), 'Sheduling elevator to', floorNum, direction);
        if (floorNum > elevator.currentFloor()) {
          elevator.switchLights('up');
        } else {
          elevator.switchLights('down');
        }
        elevator.goToFloor(floorNum);
      };
      elevator.continue = function() {
        if (elevator.destination === elevator.currentFloor()) {
          console.log(elevator.description(), 'Reached destination on', elevator.currentFloor(), 'switching light to:', elevator.direction, 'check queue:', elevator.destinationQueue);
          elevator.switchLights(elevator.direction);
          if (elevator.loadFactor() === 1){
            elevator.moveInternally();
          }
        };
      };
      elevator.getInternalDestination = function() {
        var current = elevator.currentFloor();
        var floorsBetween = function(target) { return elevator.getPressedFloors().filter( function(pressed){ return pressed < Math.abs(target - current) }) }
        return elevator
          .getPressedFloors()
          .sort(function(a, b){ return Math.abs(b - current) - Math.abs(a - current)})
          .pop();
      }
elevator.moveInternally = function(){
        var internalDestination = elevator.getInternalDestination();
        if (internalDestination !== undefined) {
          console.log(elevator.description(), 'There are still people inside, best destination:', internalDestination);
          elevator.navigateTo(internalDestination);
        }
        return internalDestination !== undefined
      }
      elevator.moveExternally = function(){
        var busyFloor = getBusyFloor(elevator.currentFloor());
        if (busyFloor && busyFloor.buttonStates.up === 'activated') {
          console.log(elevator.description(), 'No people inside, but there is some floor waiting:', busyFloor.floorNum(), 'up');
          elevator.navigateTo(busyFloor.floorNum(), 'up');
          return true;
        } else if (busyFloor && busyFloor.buttonStates.down === 'activated'){
          console.log(elevator.description(), 'No people inside, but there is some floor waiting:', busyFloor.floorNum(), 'down');
          elevator.navigateTo(busyFloor.floorNum(), 'down');
          return true;
        } else {
          return false;
        }
      }
      elevator.on("idle", function() {
        console.log(elevator.description(), 'Idle triggered for');
        elevator.destination = null;
        elevator.direction = null;
        console.log(elevator.description(), 'State cleared');
        var moved = elevator.moveInternally();
        if (!moved) { elevator.moveExternally() };
      });
      elevator.on("passing_floor", function(floorNum, direction) {
        if (elevator.isFloorRequestedInside(floorNum)) {
          console.log(elevator.description(), 'Stopping because requested from inside elevator', floorNum)
          elevator.goToFloor(floorNum);
        }
        if (isFloorRequestedOutside(floorNum, elevator.destinationDirection())){
          console.log(elevator.description(), 'Stopping at requested from ouside floor', floorNum)
          elevator.goToFloor(floorNum);
        }
      });
      elevator.on("stopped_at_floor", function(floorNum) {
        console.log(elevator.description(), 'Stopped at', floorNum);
        elevator.continue();
      })
      elevator.on("floor_button_pressed", function(floorNum) {
        console.log(elevator.description(), 'New button pressed', floorNum);
        if (elevator.isIdle()) {
          elevator.moveInternally();
        }
      })
    })
    floors.forEach(function(floor){
      floor.on("up_button_pressed", function() {
        var elevator = getIdleElevator(floor.floorNum(), 'up');
        if (elevator) {
          console.log('UP pressed on', floor.floorNum(), 'found idle elevator: ', elevator.description());
          // for best moves metric this should be commented out:
          elevator.navigateTo(floor.floorNum(), 'up');
        }
      });
      floor.on("down_button_pressed", function() {
        var elevator = getIdleElevator(floor.floorNum(), 'down');
        if (elevator) {
          console.log('DOWN pressed on', floor.floorNum(), 'found idle elevator: ', elevator.description());
          elevator.navigateTo(floor.floorNum(), 'down');
        }
      });
    });
  },
    update: function(dt, elevators, floors) { /* We normally don't need to do anything here */ }
  }
NIVEL 12 AL 14
  {
  init: function(elevators, floors) {

    var lastElevatorUsed = 0;
    var powersaving = false;    var lastCalls = [];
    sendOneElevatorTo = function(floor) {
      var cargo = 1; var emptier = [0];
      for (var e = 0; e < elevators.length; e++) {
        if (elevators[e].destinationQueue.indexOf(floor) != -1) {
          lastCalls.push(floor);
          return;
        }
        if (elevators[e].loadFactor() < cargo) {
          cargo = elevators[e].loadFactor();
          emptier = [e];
        } else if (elevators[e].loadFactor() == cargo) {
          emptier.push(e);
        }
      }
      var result = 0;
      if (emptier.length == 1) { 
        result = emptier.pop(); 
      }
      else {
        var shortestQueue = 0; var qlength = 100;
        for (var p = 0; p < emptier.length; p++) {
          var l = elevators[emptier[p]].destinationQueue.length;
          if (l<qlength) {
            l = qlength;
            shortestQueue = p;
          }
        }
        result=emptier[shortestQueue];
      }
      sendElevatorTo(elevators[result],floor);
    }
    sendElevatorTo = function(elevator, floor) {
      if (typeof(floor) == 'undefined') return;
      // elevado
      if (elevator.destinationQueue.indexOf(floor) != -1) return;
   elevator.goToFloor(floor);
    }
    // elevator eventos
    var functioningElevators = elevators.length;
    if (powersaving) functioningElevators = 1;
    for (var e = 0; e < functioningElevators; e++) {
      var elevator = elevators[e];
      elevator.on("idle", function() {
        sendElevatorTo(this,lastCalls.pop());
        });
      elevator.on("floor_button_pressed", function(floor) {
        sendElevatorTo(this,floor);
      });
      elevator.on("stopped_at_floor", function(floorNum) {
        var queue = this.destinationQueue;
        if (queue.length > 0) {
          // this.currentFloor();
        }
      });
    }
    // evento piso
    for (var f = 0; f < floors.length; f++) {
      var floor = floors[f];
      floor.on("up_button_pressed down_button_pressed", function() {
        sendOneElevatorTo(this.floorNum());
      });
    }
  },
  update: function(dt, elevators, floors) {
  }
}
<!-- Global site tag (gtag.js) - Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=UA-141698790-1"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'UA-141698790-1');
</script>
