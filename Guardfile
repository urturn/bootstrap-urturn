guard 'less', :all_on_start => true, :all_after_change => true do
  watch(%r{^.+\.less$})
end

# guard-rackup
# Tha command for rackup
#   :command => "rackup ./config.ru -E development",
#
# start(run :command as above) proc, it must return pid
#   :start => proc{ Process.spawn(command) },
#
# stop proc
#   :stop => proc{|pid| Process.kill("INT", pid); Process.wait pid},
#
# reload proc that fired when watched files changed
#   :reload => proc{ stop; start },
guard "rackup" do
  watch(%r{^urturn-theme/css/.*$})
  watch(%r{^urturn-theme/images/.*$})
  watch("config.ru")
  watch("index.html")
end
