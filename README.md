# SKTextureGradient

[![Version](https://img.shields.io/cocoapods/v/SKTextureGradient.svg?style=flat)](http://cocoadocs.org/docsets/SKTextureGradient)
[![License](https://img.shields.io/cocoapods/l/SKTextureGradient.svg?style=flat)](http://cocoadocs.org/docsets/SKTextureGradient)
[![Platform](https://img.shields.io/cocoapods/p/SKTextureGradient.svg?style=flat)](http://cocoadocs.org/docsets/SKTextureGradient)

Simple <i><a href="https://developer.apple.com/library/prerelease/ios/documentation/SpriteKit/Reference/SKTexture_Ref/index.html">SKTexture</a></i> extension for creating gradient effect in <i><a href="https://developer.apple.com/spritekit/">SpriteKit</a></i>.

# Installation

<b>CocoaPods:</b>
<pre>
Swift 2.2:
pod 'SKTextureGradient', '~> 0.1'

Swift 2.3:
pod 'SKTextureGradient', '~> 2.3'

Swift 3.0:
pod 'SKTextureGradient', '~> 3.0'
</pre>

<b>Manual:</b>
<pre>
Copy <i>SKTextureGradient.swift</i> to your project.
</pre>

# Using
<pre>
let topColor = CIColor(rgba: "#71B280")
let bottomColor = CIColor(rgba: "#134E5E")

let texture = SKTexture(size: CGSizeMake(200, 200), color1: topColor, color2: bottomColor, direction: GradientDirection.Up)
texture.filteringMode = .Nearest

let sprite = SKSpriteNode(texture: texture)
sprite.position = CGPointMake(CGRectGetMidX(frame), CGRectGetMidY(frame))
sprite.size = self.frame.size
addChild(sprite)
</pre>

# Example

![alt tag](https://raw.github.com/maximbilan/SKTextureGradient/master/example.png)

## License

SKTextureGradient is available under the MIT license. See the LICENSE file for more info.
