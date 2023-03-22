
# Rotating

### General

Q = -90
E = +90

int rotation = 0;

public void OnRotate(InputAction.CallbackContext obj)
{
  int rotateBy = obj.ReadValue< int >();
  rotation += rotateBy;

  if (rotation < -180 || rotation > 180) 
  {
	  rotation = -rotateBy;

  }
}


### Rotation for camera

### Rotation for controls