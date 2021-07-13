# Surround Preset UI
A UI to expose surround preset values in the Blender Video Sequence Editor for the various channel options.

# How to
Search for the filenames in an installed Blender 3.0 Alpha er replace the files.

# Help needed to confirm or correct these values:

    if audio_channels == 'STEREO':
      if self.stereo == 'LEFT': sequence.pan = -1
      if self.stereo == 'CENTER': sequence.pan = 0
      if self.stereo == 'RIGHT': sequence.pan = 1

    if audio_channels == 'SURROUND4':
      if self.surround4 == 'FRONTLEFT': sequence.pan = -1
      if self.surround4 == 'FRONTCENTER': sequence.pan = 0
      if self.surround4 == 'FRONTRIGHT': sequence.pan = 1

      if self.surround4 == 'REARLEFT': sequence.pan = -2 # ?
      if self.surround4 == 'REARRIGHT': sequence.pan = 2 # ?

    if audio_channels == 'SURROUND51':
      if self.surround51 == 'FRONTLEFT': sequence.pan = -1
      if self.surround51 == 'FRONTCENTER': sequence.pan = 0
      if self.surround51 == 'FRONTRIGHT': sequence.pan = 1

      if self.surround51 == 'SIDELEFT': sequence.pan = -1.250
      if self.surround51 == 'SIDECENTER': sequence.pan = 0 # ?
      if self.surround51 == 'SIDERIGHT': sequence.pan = 1.250

      if self.surround51 == 'REARLEFT': sequence.pan = -2 # Centered?
      if self.surround51 == 'REARCENTER': sequence.pan = 0 # ?
      if self.surround51 == 'REARRIGHT': sequence.pan = 2 # Centered?

    if audio_channels == 'SURROUND71':
      if self.surround71 == 'FRONTLEFT': sequence.pan = -0.33335
      if self.surround71 == 'FRONTCENTER': sequence.pan = 0
      if self.surround71 == 'FRONTRIGHT': sequence.pan = 0.33335

      if self.surround71 == 'SIDELEFT': sequence.pan = -1.66667
      if self.surround71 == 'SIDECENTER': sequence.pan = 0 #?
      if self.surround71 == 'SIDERIGHT': sequence.pan = 1.66667

      if self.surround71 == 'REARLEFT': sequence.pan = -1.222
      if self.surround71 == 'REARCENTER': sequence.pan = 2 # ?
      if self.surround71 == 'REARRIGHT': sequence.pan = 1.222

