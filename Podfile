platform :ios, '12.0'

target 'KnobShowcase' do
  use_frameworks!

#  pod 'KnobControl', :path => '../KnobControl'
  pod 'KnobControl', :git => 'https://github.com/talkabhishek/KnobControl.git', :tag => '1.0.1'

end

# Workaround for Cocoapods issue #7606
post_install do |installer|
    installer.pods_project.build_configurations.each do |config|
        config.build_settings.delete('CODE_SIGNING_ALLOWED')
        config.build_settings.delete('CODE_SIGNING_REQUIRED')
    end
end
