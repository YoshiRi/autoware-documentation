---
title: /api/routing/set_route_points
method: function call
type:
  name: autoware_adapi_v1_msgs/srv/SetRoutePoints
  req:
    - name: header
      text: header for pose transformation
    - name: goal
      text: goal pose
    - name: waypoints
      text: waypoint poses
  res:
    - name: status
      text: response status
---

{% extends 'design/autoware-interfaces/templates/autoware-interface.jinja2' %}
{% block description %}
Set the route with the waypoint poses. If start pose is not specified, the current pose will be used.
{% endblock %}
