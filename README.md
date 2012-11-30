# $P Point-Cloud Recognizer for Objective-C

An Objective-C port of the $P gesture recognizer to be used in iOS applications.

![Demo App](https://raw.github.com/fe9lix/DollarP_ObjC/gh-pages-data/images/dollarp-objc-demo-app.png)

## What is $P?
From the [$P website](http://depts.washington.edu/aimgroup/proj/dollar/pdollar.html):

> The $P Point-Cloud Recognizer is a 2-D gesture recognizer designed for rapid prototyping of gesture-based user interfaces. In machine learning terms, $P is an instance-based nearest-neighbor classifier with a Euclidean scoring function, i.e., a geometric template matcher. $P is the latest in the dollar family of recognizers that includes $1 for unistrokes and $N for multistrokes. Although about half of $P's code is from $1, unlike both $1 and $N, $P does not represent gestures as ordered series of points (i.e., strokes), but as unordered point-clouds. By representing gestures as point-clouds, $P can handle both unistrokes and multistrokes equivalently and without the combinatoric overhead of $N. When comparing two point-clouds, $P solves the classic assignment problem between two bipartite graphs using an approximation of the Hungarian algorithm. The $P recognizer is distributed under the New BSD License agreement.

## How to use
* All gesture recognizer classes are located in libs/DollarP. Just drag this folder into your Xcode project.
* See the code of the demo app on how to use the recognizer. GestureViewController is the class where the recognizer is added to the view...

## Notes
* You need to add additional templates to improve gesture scores (Customize/Add to existing type...)
* Custom templates are not persisted between launches!