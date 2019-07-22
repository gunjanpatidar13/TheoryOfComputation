


dfa={0:{'a':1,'b':3},
     1:{'a':0,'b':2},
     2:{'a':3,'b':1},
     3:{'a':2,'b':0}
     }
     
InitialState=0
FinalState={0}
def function(string):
    CurrentState=InitialState
    for i in string:
        CurrentState=dfa[CurrentState][i]
    if CurrentState == FinalState:
        return True
    else:
        return False
    
function('aabb')             
