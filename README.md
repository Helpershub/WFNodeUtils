/**
 * WFNodeUtils JavaScript Library v1.0
 * http://sarveshspn.blogspot.com/
 * Copyright 2012, Sarvesh Navelkar
 * Licensed under the MIT or GPL Version 2 licenses.
 * Date: Dec 12 2012
 *
 * Copyright (C) 2011 - 2012 by Sarvesh Navelkar
 *
 * Permission is hereby granted, free of charge, to any person obtaining a copy
 * of this software and associated documentation files (the "Software"), to deal
 * in the Software without restriction, including without limitation the rights
 * to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 * copies of the Software, and to permit persons to whom the Software is
 * furnished to do so, subject to the following conditions:
 *
 * The above copyright notice and this permission notice shall be included in
 * all copies or substantial portions of the Software.
 *
 * THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 * IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 * FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 * AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 * LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 * OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 * THE SOFTWARE.
 */
 
 
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
