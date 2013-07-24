require 'fileutils'

task :default => ["referaatti:build"]
task :clean => %w[referaatti:clean aine:clean esitelma:clean kandi:clean]
namespace :referaatti do
  desc "Build referaatti.tex with ../lahteet.bib"
  task :build do
    sh "cd referaatti && pdflatex referaatti && bibtex referaatti && pdflatex referaatti && pdflatex referaatti"
  end

  desc "Cleans crap generated by latex from referaatti folder"
  task :clean do
    crap = %w[referaatti.aux referaatti.bbl referaatti.blg referaatti.log referaatti.out referaatti.pdf]
    FileUtils.chdir "referaatti" do
      FileUtils.rm_rf crap
    end
  end

end

namespace :aine do
  desc "Build aine.tex with ../lahteet.bib"
  task :build do
    sh "cd aine && pdflatex aine && bibtex aine && pdflatex aine && pdflatex aine"
  end

  desc "Cleans crap generated by latex from aine folder"
  task :clean do
    crap = %w[aine.aux aine.bbl aine.blg aine.log aine.out aine.pdf]
    FileUtils.chdir "aine" do
      FileUtils.rm_rf crap
    end
  end

end

namespace :kandi do
  desc "Build kandi.tex with ../lahteet.bib"
  task :build do
    sh "cd kandi && pdflatex kandi && bibtex kandi && pdflatex kandi && pdflatex kandi"
  end

  desc "Cleans crap generated by latex from kandi folder"
  task :clean do
    crap = %w[kandi.aux kandi.bbl kandi.blg kandi.log kandi.out kandi.pdf]
    FileUtils.chdir "kandi" do
      FileUtils.rm_rf crap
    end
  end

end



namespace :esitelma do
  desc "Build esitelma.tex with ../lahteet.bib"
  task :build do
    sh "cd esitelma && pdflatex esitelma && bibtex esitelma && pdflatex esitelma && pdflatex esitelma"
  end

  desc "Cleans crap generated by latex from esitelma folder"
  task :clean do
    crap = %w[esitelma.aux esitelma.bbl esitelma.blg esitelma.log esitelma.out esitelma.pdf]
    FileUtils.chdir "esitelma" do
      FileUtils.rm_rf crap
    end
  end

end

