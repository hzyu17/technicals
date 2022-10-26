# installing drake
Need at least ubuntu20.04
## before installing, remember to run the file in [this link](https://drake.mit.edu/ubuntu.html)

### install via apt tool
refer to [this link](https://drake.mit.edu/apt.html)
This will install drake into /opt/drake

## Visualization in drake using meshcat:
install meshcat:
```
pip install meshcat
```
install zeroMQ:
```
apt install libzmq3-dev
```
starting a server:
```
meshcat-server
```
visualizing in code:
creating a MeshcatVisualizer class using a scene_graph, and add to the diagram builder. The default zmq url will be the same as the server you just created
```
meshcat_viz = MeshcatVisualizer(scene_graph)
builder.AddSystem(meshcat_viz)
builder.Connect(scene_graph.get_query_output_port(), meshcat_viz.get_geometry_query_input_port())
```
More details: [Meshcat_python](https://github.com/rdeits/meshcat-python)

## Run drake_visualizer:
after installing using apt,
```
/opt/drake/bin/drake-visualizer
```

