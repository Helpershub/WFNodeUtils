
WFNODEUTILS.Node
A Node comprises a single unit or single block in the entire workflow
Currently nodes have one or more endpoints which can be of type in or out (denoting an input
or an output endpoint.Our Node objects would contain the display Kinetic.JS objects and each 
of these Kinetic.JS objects will contain a back reference to it's container node object
as events are raised by KineticJS on KineticJS objects

WFNODEUTILS.NodeEndPoint 
A node endpoint serves as the point at which we would be connecting two nodes together.
Two nodes are connected via their endpoints

WFNODEUTILS.NodeLineConnector
A Node Connector internally contains the endpoints which it connects together using straight lines

WFNODEUTILS.NodeTemplateDisplayContainer
This container would contain the node templates, node templates are
nodes which when clicked generate actual nodes which can be connected. The Node templates
appear on the left hand side of the screen

WFNODEUTILS.NodeDisplayContainer
This contains the actual draggable nodes which can be connected and is also the parent top level
container for the NodeTemplateContainer. Events and functionality is wired up based on which container 
you add the nodes for example Nodes added to the Template Container are not draggable

WFNODEDRAWINGAPP.Main 
The Main function which generates the various Nodes
