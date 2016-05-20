source 'https://github.com/CocoaPods/Specs.git'

platform :ios, '8.0'
use_frameworks!

def core_pods
    pod 'DACircularProgress', '2.2.0'
    pod 'SDWebImage', '3.7.1'
    pod 'REFrostedViewController', '~> 2.4.7'
    pod 'FXBlurView'
    pod 'MBProgressHUD'
    pod 'MarqueeLabel'
    pod 'Parse'
    pod 'Crashlytics'
end

target 'CocoaPodsIssueTest' do
    core_pods
end

# Make all dependencies build for all architectures 
post_install do |installer|
    installer.pods_project.build_configurations.each do |config|
        config.build_settings['ONLY_ACTIVE_ARCH'] = 'NO'
    end
end
