python3.10 -m venv venv_viser && source venv_viser/bin/activate

python3 -m pip install --upgrade certifi

python3 -m pip install -e ".[examples]"
<!-- python3 -m pip install pip-system-certs -->

download and unzip data to:
```
ls examples/assets/record3d_dance
icon		metadata	rgbd		sound.m4a
```

in "src/viser/_client_autobuild.py"

use "--with-npm" when create a nodeenv.

```
        [sys.executable, "-m", "nodeenv", "--with-npm", "--node=20.4.0", env_dir], check=False
```

run scripts:
```
python examples/07_record3d_visualizer.py
```


reference:
- https://threejs.org/docs/#examples/en/controls/PointerLockControls
- https://drei.docs.pmnd.rs/controls/camera-controls
- https://github.com/yomotsu/camera-controls
- https://discourse.threejs.org/t/is-it-possible-to-disable-the-zooming-of-cameracontrols-react-three-drei/67476
- https://github.com/pmndrs/drei
- https://codesandbox.io/p/sandbox/
- https://codesandbox.io/p/sandbox/first-person-controller-82b7fs
- https://codesandbox.io/p/sandbox/r3f-first-person-navigation-tx1kog


camera controls: do i need this or PointerLockControls
- https://www.npmjs.com/package/camera-controls
- https://github.com/yomotsu/camera-controls/blob/dev/examples/first-person.html
